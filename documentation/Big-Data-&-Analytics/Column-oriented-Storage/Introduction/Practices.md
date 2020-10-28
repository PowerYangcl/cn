
# 案例分析

* A. 统一日志案例

 场景:写多读少,写入量巨大(日写入>37 亿),读取随机且访问较少。

 设计:将 Rowkey 用 UUID 类似方式生成随机字段,转换成 Byte 数组,经过优化,截取为 4 个 Byte。既随机,又很短,能满足 40 年存储。通过 HBase 组针对性的预分区,将数据区域划分到所有节点上,写入均衡到每个节点,因此压力平均。读取的时候,因为随机,设置了 BLOOMFILTER,所以随机读性能提高。因为读取少,所以对于读取的优化就没有写那么重要了。

* B. 一次导入,多次读取

 场景:晚上导入大量数据,白天提供用户访问,每次查询是带有客户 ID 的随机数据,数据量可以估算,每条数据<100B。

 设计:晚上导入大量数据,如果只有一台服务器提供服务,TPS 上不去,且容易导致节点宕机,因此需要写入是均衡分布的。另外一方面,用户访问的时间和方式是比较随机的,数据又是随机的,因此将 Rowkey随机分布有助于大量请求比较均衡在多个节点上。因为用户的访问更重要,因此将客户 ID 和相关业务类型作为 Rowkey。如果写入数据是对用户顺序处理的,就会出现压力集中在某个节点上,导致宕机。于是将导入 worker 设计为先在本地存储,然后分 10 个线程,将用户 Hash 成 10 组。每个线程读取一个用户的 300条数据,批量写入 HBase,然后写下一个用户的 300 条数据,继续直到第 10 个用户,再返回写本组第一个用户,直到所有数据写完。最终集群的表现比较平稳,且 TPS 很高。

* C. 监控数据(京东云容器监控cap，京东大脑，jdh监控，bdp监控数据查询,ump,mjdos)

* D. 海量存储（商家罗盘，供应商罗盘，Storm实时应用，搜索推荐)
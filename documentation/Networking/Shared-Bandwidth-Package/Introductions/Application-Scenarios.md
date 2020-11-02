# 应用场景

### 业务量大

随着业务增长，大量的业务需要布置在云上，每个云主机、容器等实例均需要单独使用一条带宽，可通过将同一个项目中的公网IP资源加入一个共享带宽包实现根据业务对资源进行分组管理


### 业务多样化

不同公网IP绑定资源提供的服务时间不一样，例如某个公网IP绑定的资源主要在白天提供服务，另外一个公网IP绑定的资源主要用于晚间服务，这两个公网IP需要的带宽上限均为200Mbps，可将这两个公网IP加入带宽上限为300Mbps的共享带宽包，共用一条带宽，不仅会极大地降低带宽费用成本，还方便运维统计。



### 业务爆发式访问

共享带宽包支持消峰计费，可支持短时间内带宽爆发式增长的业务，在突发流量外，其余时间整体带宽速率较低，如电商促销活动、限时秒杀等，采用消峰计费模式，短时间的突发流量费用不计入带宽费用，降低带宽成本。

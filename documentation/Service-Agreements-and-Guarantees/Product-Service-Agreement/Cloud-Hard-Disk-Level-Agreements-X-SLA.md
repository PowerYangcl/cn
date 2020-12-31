**版本生效日期：2021年1月1日**

**1.服务范围**

京东智联云云硬盘是利用京东在分布式存储领域多年的深厚技术积累，为用户提供的低时延、高可靠、高可用块存储服务。云硬盘的数据以三副本方式存储，避免因组件故障影响数据完整性。云硬盘容量可弹性扩展，同时支持快照和自定义快照策略功能。目前云硬盘包含预付费和后付费两种结算方式。

**2.服务等级指标**

**2.1数据持久性**

数据持久性：不低于99.9999999%；

数据持久性按服务周期统计，一个服务周期为一个自然月，如不满一个月不计算为一个服务周期。

**2.2数据可销毁性**

2.2.1．在用户主动删除数据或用户服务期满后需要销毁数据的，京东智联云将自动清除对应物理服务器上磁盘和内存数据，使得数据无法恢复。

2.2.2．云服务所用的设备在报废弃置、委外维修或转售前，京东智联云将对其物理磁盘采用消磁操作。

**2.3数据可迁移性**

用户使用云硬盘时，可通过使用虚机、容器等计算产品挂载云硬盘的方式，访问其云硬盘中的数据。当数据需要迁移时，可通过工单申请方式，申请以云硬盘快照的形式进行导出。

**2.4数据私密性**

用户可在京东智联云官网开通云硬盘服务。用户仅在京东智联云完成登录，用户身份校验通过的情况下，才可以操作云硬盘并访问其中的数据。不同用户间的云硬盘数据是相互隔离的。

京东智联云提供了“加密”盘功能，采用AES-256算法对云硬盘数据进行加密，可以进一步保障用户的数据私密性。

**2.5数据知情权**

2.5.1．用户对于数据、备份数据所在数据中心地理位置、数据备份数量具有知情权，其中：

2.5.1.1．目前京东智联云数据中心分别位于华北（北京）、华东（宿迁）、华东（上海）和华南（广州），用户在开通云服务时必须根据地理位置选择相应的数据中心，用户数据将存储在其指定的数据中心；

2.5.2．京东智联云的数据中心将遵守当地的相关法律法规，用户对此具有知情权，并可联系京东智联云的客户服务人员获得详尽信息。

2.5.3．除应当地法律法规、或政府监管部门的监管、审计要求，用户的所有数据、应用及行为日志不会提供给第三方。除用于京东智联云的产品运行状态的统计分析，用户的行为日志不会对外呈现用户个人信息数据。

**2.6数据可审查性**

依据现行法律法规或根据政府监管部门监管、安全合规、审计或取证调查等原因的需要，在符合流程和手续完备的情况下，京东智联云可以提供用户所使用的服务的相关信息，包括关键组件的运行日志、运维人员的操作记录、用户操作记录等信息。

**2.7服务功能**

京东智联云提供提供通用型SSD云硬盘、性能型SSD云硬盘和容量型HDD云硬盘三种云硬盘选项，满足不同性能要求的业务场景。

容量型HDD云盘：单盘容量：20-16000G；不承诺最大IOPS和最大吞吐量。典型应用场景：可用于读写速率适中、事务性处理较少、冷数据备份等场景； 

通用型SSD云盘：单盘容量：20-16000G；单盘最大IOPS：15000；单盘最大吞吐量：150MBps；典型应用场景：引导卷、小型数据库、大型开发测试、web服务器以及其它需要随机读写的业务场景； 

性能型SSD云盘：单盘容量：20-16000G；单盘最大IOPS：32000；单盘最大吞吐量：150MBps；典型应用场景：大数据分析、I/O密集型业务、 中大型数据库应用。

云硬盘提供高可靠、高可用、高性能的数据存储服务：1）云硬盘数据独立于云主机状态，支持随时挂载和卸载操作，单台云主机最多可挂载8块云硬盘（包含系统盘），满足用户更高的存储需求；2）用户只需要为云硬盘的当前容量和类型付费，并可以随时根据业务发展扩充云硬盘容量；3）提供云硬盘IOPS和吞吐量实时监控，随时掌握硬盘健康状态。

云硬盘提供快照功能以实现指定时间点的数据备份

1）快照是对云硬盘的完全拷贝，包含磁盘自创建至备份时间点的数据映像，以冗余的方式存储。 2）您可通过快照对云盘做回滚操作，让您的业务恢复到任一快照时间点。 3）对云主机制作镜像，可同时对挂载到云主机的云硬盘创建快照，基于云主机镜像，可快速复制相同配置的云主机，实现业务快速批量部署。

**2.8服务可用性**

服务可用性：不低于99.95%。

云硬盘服务可用性计算公式为：每服务周期单个云硬盘实例所有可用时间/（每服务周期单个云硬盘实例所有可用时间＋每服务周期单个云硬盘实例所有不可用时间）。

云硬盘可用性按服务周期统计，一个服务周期为一个自然月，如不满一个月不计算为一个服务周期。

统计的业务单元为每个用户的所有云硬盘实例，时间单位为分钟。

不可用时间：云硬盘所提供的服务在连续的5分钟或更长时间不可使用方计为不可用时间，不可使用的服务时间低于5分钟的，不计入不可用时间，云硬盘不可用时间不包括日常系统维护时间、由用户原因、第三方原因或不可抗力导致的不可用时间。

**2.9故障恢复能力**

京东智联云为付费用户的云服务提供7×24小时的运行维护，并以在线工单和电话报障等方式提供技术支持，具备完善的故障监控、自动告警、快速定位、快速恢复等一系列故障应急响应机制。

**2.10服务计量准确性**

京东智联云云硬盘具备准确、透明的计量计费系统，京东智联云根据用户的京东智联云云硬盘购买容量大小据实结算，具体计费标准以京东智联云官网公布的有效的计费模式与价格为准。用户的原始计费日志默认最少保留1年备查。

**2.12** **服务赔偿条款**

2.12.1 赔偿范围：

因京东智联云故障导致云硬盘无法正常使用，以及京东智联云故障引起的网站无法正常访问，京东智联云将对不可用时间进行赔偿，但不包括以下原因所导致的服务不可用时间：

1、京东智联云预先通知用户后进行系统维护所引起的，包括割接、维修、升级和模拟故障演练；

2、由于运营商故障导致的丢包和延时等不可用情况；

3、用户的应用程序或数据信息受到黑客攻击而引起的；

4、用户维护不当或保密不当致使数据、口令、密码等丢失或泄漏所引起的；

5、用户自行升级操作系统所引起的；

6、用户的应用程序或安装活动所引起的；

7、用户的疏忽或由用户授权的操作所引起的；

8、不可抗力以及意外事件引起的；

9、其他非京东智联云原因所造成的不可用。

2.12.2. 赔偿方案

根据客户某一京东智联云账号下云硬盘的地域及存储类型分别统计 **月度** 服务可用性，按照下表中的标准计算赔偿金额。赔偿方式仅限于用于支付云硬盘产品的 **代金券**，且赔偿总额不超过未达到服务可用性承诺的当月 **该地域下该存储类型**所支付月度服务费用总额的100%（ **不含用代金券抵扣的费用**）。 

 

| **可用性**            | **赔付标准**     |
| --------------------- | ---------------- |
| 99.95%>可用性>=99.00% | 月度服务费的15%  |
| 99.00%>可用性>=95.00% | 月度服务费的30%  |
| 可用性<95.00%         | 月度服务费的100% |

 

**3.** **其他**

京东智联云有权根据变化适时对本服务等级协议部分服务指标作出调整，并及时在京东智联云官网（[www.jdcloud.com](https://www.jdcloud.com/)）发布公告或发送邮件或书面通知向用户提示修改内容。

 
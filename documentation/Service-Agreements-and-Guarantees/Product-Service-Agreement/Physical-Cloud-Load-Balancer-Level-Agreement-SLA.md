### 1.服务范围

本服务等级协议（Service Level Agreement，以下简称 “SLA”）规定了京东智联云向客户提供物理云负载均衡（Elastic Load Balancer，简称“ELB”）的服务可用性等级指标及赔偿方案，京东智联云的其他负载均衡产品不在本服务等级协议覆盖范围内。

### 2.服务等级指标

#### 2.1 服务功能

京东智联云提供的物理云负载均衡服务，旨在通过流量分发控制将前端访问的大并发流量按照用户要求分发到多台后端实例，专用于云物理服务器；主要功能包括创建和管理负载均衡实例、创建和管理监听器、配置监听端口、配置健康检查、配置会话保持等。

#### 2.2服务可用性
服务周期：一个服务周期为一个自然月，如不满一个自然月不计算为一个服务周期。

服务周期分钟数：指按照一个服务周期内实际总天数×24（小时）×60（分钟）计算所得的分钟时长。

服务周期不可用分钟数：指一个服务周期内单用户的单个负载均衡实例的所有监听的服务不可用累计分钟时长。

服务可用性计算公式：（一个服务周期内单用户单地域所有可用区内所有负载均衡实例的服务周期分钟数之和 – 一个服务周期内单用户单地域多可用区内所有负载均衡实例的服务周期不可用分钟数之和）/（一个服务周期内单用户单地域所有可用区内所有负载均衡实例的服务周期分钟数之和）×100%。

服务可用性承诺：一个服务周期内单用户单地域的服务可用性不低于99.9%。

（地域：指的是京东智联云的Region概念；可用区：指的是京东智联云的AZ概念。）

#### 2.3故障恢复能力

京东智联云为付费用户的物理云负载均衡实例提供7×24小时的运行维护，并以电话报障等方式提供技术支持，具备完善的故障应急响应机制。

#### 2.4网络接入性能

用户在开通京东智联云物理云负载均衡服务时，可自主选择为每个负载均衡实例配置所需的公网出口带宽（通过绑定物理云公网IP），公网出口带宽可配置的范围从1Mbps至200Mbps。

#### 2.5服务计量准确性

物理云负载均衡服务具备准确、透明的计量计费系统，京东智联云根据用户的物理云负载均衡实例的计费类型、实际使用时长和购买数量进行扣费结算。具体计费&扣费标准以京东智联云官网公布的有效的计费模式、价格和扣费方法为准。用户的原始计费日志默认最少保留1年备查。

### 3、服务赔偿条款

#### 3.1 赔偿范围

因京东智联云设备故障、设计缺陷或操作不当导致客户所购买的物理云负载均衡服务无法正常使用，京东智联云将对不可用时间进行赔偿，但不包括以下原因所导致的服务不可用时间：

（1）京东智联云预先通知用户后进行系统维护所引起的，包括割接、维修、升级和模拟故障演练；

（2）任何京东智联云所属设备以外的网络、设备故障或配置调整引起的；

（3）客户的应用程序受到黑客攻击而引起的，包括但不限于在遭到DDoS攻击时，公网IP被京东智联云设置为黑洞状态或清洗状态；

（4）客户配置错误（例如，错误配置防火墙、监听端口、证书等原因）导致服务不可用；

（5）客户未配置后端服务器或后端服务器异常导致的问题（建议用户打开健康检查功能，实时监测后端服务器的状态）；

（6）客户未遵循京东智联云产品使用文档或使用建议引起的；

（7）客户的疏忽或由客户授权不当的操作所引起的；

（8）不可抗力以及意外事件引起的；

（9）由于客户违反《京东智联云服务协议》导致的物理云负载均衡服务被暂停或终止，包括但不限于由于订单过期或者账号欠费导致负载均衡实例被暂停服务或被释放等；

（10）其他非京东智联云原因所造成的不可用。

#### 3.2 赔偿方案

故障时间=不可用时间。

包年包月的物理云负载均衡以服务时长补偿的方式，按故障时间100倍/单个实例赔偿。

说明：

京东智联云通过赠送代金券的方式进行赔偿，赠送代金券仅供支持购买物理云负载均衡产品，赔偿总额不超过当月用户就该物理云负载均衡实例已支付的月度服务费用（不含赠送金额或者代金券抵扣的费用）；

物理云负载均衡只赔偿物理云负载均衡实例自身，不赔偿物理云负载均衡实例关联的云物理服务器。

### 4. 其他

京东智联云有权根据变化适时对本服务等级协议部分服务指标作出调整，并及时在京东智联云官网[www.jdcloud.com](https://www.jdcloud.com) 发布公告或发送邮件或书面通知向用户提示修改内容。如您不同意京东智联云对本服务等级协议所做的修改，您有权停止使用物理云负载均衡服务，如您继续使用物理云负载均衡服务，则视为您接受修改后的服务等级协议。
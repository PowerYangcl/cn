## 功能问题

1.消息队列Kafka版支持外网访问吗？</br>

为提升数据访问的安全性，消息队列Kafka版目前仅支持用户VPC内访问。可以通过创建和Kafka实例处于同一VPC内的云主机实现外网访问。</br>

2.可以访问部署消息队列Kafka版的机器吗？</br>

不可以，消息队列Kafka版作为全托管服务，用户无需维护所有基础设施，包括操作系统更新和其他日常维护。</br>

3.当前消息队列Kafka版基于开源哪个版本？</br>

当前消息队列Kafka版基于 Apache Kafka V1.0.2和V0.10.2 版本，推荐生产消费端选取对应版本的 SDK。</br>

4.Kafka为什么使用消费者组？</br>

消费者组保证了：</br>
-	一个分区只可以被消费组中的一个消费者所消费。</br>
-	一个消费组中的一个消费者可以消费多个分区。</br>
-	一个消费组中的不同消费者消费的分区一定不会重复。</br>
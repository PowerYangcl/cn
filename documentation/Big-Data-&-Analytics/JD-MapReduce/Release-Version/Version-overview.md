# 版本概述

京东智联云弹性MapReduce（JMR）由一系列大数据生态的开源应用程序组成。每个JMR的版本，包含了一组特定版本的开源程序。当您在创建集群时，可以选择对应的JMR版本，以满足您对其中包含的开源组件的版本需求。

### 产品版本号格式

弹性MapReduce采用类似 **JMR-a.b.c**格式的版本号，详细说明如下：

- a 代表当前版本支持的 Hadoop 版本，如a 等于2为支持 Hadoop 为2.X版本。
- b 代表版本中一些组件的变动，即新增组件或对一些组件的版本进行了升级。
- c 代表版本中的bug修复、功能优化，可以向前兼容。

注意：

- 每个JMR版本上捆绑的组件和组件版本都是固定的。目前不支持组件的多个不同版本的选择，也不推荐您自行更改组件的版本。
- 当选择了JMR某个版本创建集群后，该集群使用的 JMR 版本和组件版本不会自动升级。后续即使对JMR版本进行了升级，也不会影响已经创建的集群。只有新的集群才会使用新的镜像。
- 当升级集群版本时（例如，从 JMR-V2.0.0 版本升级到 JMR-V2.1.0 版本），为防止一些升级不兼容、环境变化等问题的出现，请务必测试集群中的作业，以确保在新的软件环境中可以正常运行。

### 产品发行版本

| 组件名称      | JMR-2.0.0 | JMR-2.1.0 |
| ------------- | --------- | --------- |
| 发布时间      | 2018.03   | 2020.11   |
| Hadoop        | 2.7.4     | 2.8.5     |
| Hive          | 2.1.1     | 2.3.7     |
| Spark         | 2.2.0     | 2.4.7     |
| Knox          | -         | -         |
| Tez           | 0.9.1     | -         |
| Ganglia       | 3.7.2     | 3.7.2     |
| Hue           | 4.0.0     | 4.0.0     |
| HBase         | 1.2.6     | 2.2.4     |
| ZooKeeper     | 3.4.10    | 3.4.10    |
| Presto        | 0.187     | 0.187     |
| Phoenix       | 4.12.0    | 5.0.0     |
| Flink         | -         | 1.10.0    |
| Oozie         | 4.3.1     | 4.3.1     |
| Sqoop         | 1.4.6     | 1.4.6     |
| Zeppelin      | 0.7.3     | 0.8.2     |
| Alluxio       | 1.6.0     | 1.6.0     |
| Kafka         | 0.11.0    | 0.11.0    |
| ElasticSearch | 5.6.2     | 5.6.2     |

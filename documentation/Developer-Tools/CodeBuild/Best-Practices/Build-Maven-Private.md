# 在Maven工程中使用京东云制品库

本文档提供在云编译上使用京东云制品库的例子。


基本操作流程如下：

1）在京东云-代码托管中创建源代码

2）在京东云-制品库中创建用户私库

3）在京东云-制品库中上传私有依赖包

4）在京东云-制品库中下载私库settings文件，并且上传到示例代码库中，修改构建脚本指定settings文件

5）在京东云-云编译中，对示例代码进行构建，构建过程中下载私有依赖包


### 将代码上传至代码托管

京东云的代码托管服务地址为：https://code.jdcloud.com/

### 在制品上传私有依赖包，获取私库配置

**一、在私库中上传私有依赖包**
 1. 参考制品库，[制品管理-上传制品](https://docs.jdcloud.com/cn/artifacts/manage-artifacts)

**二、在使用指南中下载settings文件**
 1. 参考制品库，[用户私库-使用指南](https://docs.jdcloud.com/cn/artifacts/private)

### 修改代码

1) 将settings.xml上传至代码库根目录

2) 修改构建脚本使用仓库中的settings.xml进行构建

### 在云编译中创建编译任务

云编译任务列表页面，点击 新建任务。

具体信息如下：

   ![](/image/codebuild/best-maven-jobconf.png)
   
构建命令中增加指定settings.xml的命令：

   ![](/image/codebuild/best-maven-settings.png)

在pom.xml文件中增加对私库包的依赖

   ![](/image/codebuild/best-deps.png)

保存并执行，编译构建任务。

 
### 查看构建日志

在任务详情页面可以查看最新的构建日志，也可以下构建历史中查看历次的构建历史。
可以看到从私库中下载了私有依赖包。

   ![](/image/codebuild/best-maven-dl.png)


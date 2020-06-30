# 修改订阅任务

订阅任务正常运行时，如需要修改订阅任务，修改信息包括：源库、目标端、订阅对象。

## 注意事项

- 修改订阅任务后，数据订阅服务将重新从源数据库获取数据或结构更新，原有数据与进度将不做保存。

## 操作步骤

1. 登录 [DTS 控制台](http://dts-console.jdcloud.com/subscription/list)，在左侧菜单点击**数据订阅**。

2. 在数据订阅列表页，选择目标任务，在操作项中点击**修改订阅任务**。

   ![image-20200629121033812](D:\MD\DTS\帮助文档\image\Data-Transmission-Service\dts-030.png)

   或者进入任务详情页，点击**操作-修改订阅任务**。

   ![image-20200629144329976](D:\MD\DTS\帮助文档\image\Data-Transmission-Service\dts-034.png)

3. 在“修改订阅任务”页面填写相应信息，请参考“[配置订阅任务](Config-Subscription-Task.md)”。

4. 修改完成后，等待任务完成预检查并正常运行。
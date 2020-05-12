# 事件订阅

## 基本信息设置

1. 输入订阅规则名称，必填项

2. 根据需求输入对订阅规则的描述，选填项

## 事件源设置

1. 选择事件来源类型，选择系统事件

2. 选择事件来源，选择云监控

3. 事件类型，选择资源监控报警

4. 事件筛选未非必填项，选择资源监控类型-全部类型

5. 订阅对象，选择全部对象或者选择部分报警规则

## 事件目的地设置

1. 选择云主机重启API

2. 选择指定地域的某台云主机

点击**确定**完成订阅规则的设置。设置完成后，默认开启订阅。

当订阅对象中选择的报警规则发生告警时，指定的云主机进行重启，若报警未恢复，则云主机会不断进行重启。

![](https://raw.githubusercontent.com/jdcloudcom/cn/zhangwenjie-only/image/CloudEvents/createCE01.jpg)


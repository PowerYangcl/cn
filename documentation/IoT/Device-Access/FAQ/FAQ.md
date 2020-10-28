# 常见问题

**Q：设备上报了一个事件，但是数据概览页的上报事件曲线仍显示为0，为什么？**

A：上报事件曲线图中显示的是昨天的数据，今天上报的事件需要等明天才能看到。
比如，当前页面曲线上，横坐标8:00对应的事件个数为10，表示昨天 (7:00 , 8:00]之间所有事件的总数为10。

**Q：新增连接代理设备类型的物模型，系统自带了一个模型“连接代理模型”。我不想要这个模型，有办法删除吗？**

A：此模型不允许删除和修改。如果该模型不满足要求，可以在模型列表中新增一个模型来添加其他的属性. 方法. 事件。

**Q：新建连接代理设备的物类型后，有个通讯协议档案tab是必填吗，怎么填？**

A：是非必填。

**Q：连接代理设备在添加代理关系时报错，怎么排查？**

A：报错主要有以下2种原因：
a)连接代理设备不在线。解决办法：先将连接代理设备上线，然后再关联。
b)被添加的非直连设备被其他连接代理设备关联过。解决办法：先接触非直连设备之前的关联关系，然后再添加。

**Q：打开设备的属性tab页面， 能看到设备的属性值，但属性值对应的期望值列不允许填写，怎么办？**

A：查看该属性的权限值，如果权限是“r”,说明该属性值是只读的，不允许修改是正常的。
对于想下发期望值的属性，需要在新建物模型的时候就将属性值设置为rw或w。

**Q：非直连设备怎么上线？**

A：
a) 找到非直连设备要挂载的连接代理设备，将其上线
b)打开连接代理设备的拓扑tab，添加代理关系，关联该非直连设备
c)点击下发拓扑按钮
d)检查非直连设备状态，由未激活变成了在线

**Q：设备分组关联该设备时，点击添加设备按钮，设备列表为空。**

A：设备分组是子分组时，仅可以关联其父分组已关联过的设备。如果父分组未关联任何设备，则子分组在关联设备时的列表就是空的。

**Q：设备分组关联该设备时，点击添加设备按钮，设备列表中没有找到设备A。**

A：设备分组是子分组时，仅可以关联其父分组已关联过的设备。如果父分组没有关联过设备A，则子分组关联设备时的列表中就没有设备A。可以先在父分组中关联设备A，然后子分组再关联。

**Q：新建规则引擎时的类SQL语句的表名是固定的吗？**

A：不是固定写死的。举例：select * from aaa where timestamp > 1592289113。其中表名“aaa”可以填写任意字符串，过滤时只参考where后的条件部分。

**Q：新建规则引擎时的设备上报数据必须跟上报的payload内容一模一样吗?**

A：不需要。上报数据可以是payload的内容，也可以是只填写payload中部分参数值

**Q：规则引擎想用kafka（或mysql/JCQ），怎么申请kafka（或mysql/JCQ）地址？**

A：使用京东云账号登陆kafka控制台（或mysql/JCQ的控制台），点击新建按钮。
注意：新建kafka和mysql时的地域和私有网络必须跟物联管理平台实例的一致，JCQ只需要地域选项一致即可。详细步骤可参考使用手册的规则引擎部分。

**Q：档案列表是做什么的，是会必须用到吗？**

A：档案可以理解为新增页面的一个填写选项，是方便用户扩充新增物类型（或设备）页面字段设定的，不一定会用到。如果系统中新增物类型（或设备）页面中的字段信息已足够用，就不需要用到该功能。

**Q：档案中物类型设备选项有什么作用？**

A：新建档案页面，如果选择物类型会有个物类型字段，是必填的。档案添加成功后，则新建设备时，如果选择此物类型，页面会自动增加一个档案字段；如果选择其他物类型，则不增加。


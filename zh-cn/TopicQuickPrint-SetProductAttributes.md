## 从零开始设置一个产品属性

> 这里讲述从零基础了解OPS中的产品属性的作用以及创建。

### 产品属性是什么？

> 是指从印前到印刷所遇到各种“参数”；

**这些参数可以是：**
- 印刷设备
- 产品工艺
- 纸张类型
- 快递信息
- 下单数量
- ……

我们通过这些参数信息我们系统串联起来，成为通用的产品属性。

### 是如何工作的 ？

> 设计一个产品通过需求，应用不同的印刷工艺以及各项细节进行关联，可以使得客户可以自定义选择下单；
> 

效果如下截图：
<!-- tabs:start -->

<!-- tab:前台应用截图 -->
<center><img src="/zh-cn/images/Topic/list24.png" alt="img" style="zoom:100%;" /></center>

<!-- tab:后台所有产品属性 -->
<center><img src="/zh-cn/images/ProductManagement/list9.png" alt="img" style="zoom:100%;" /></center>

<!-- tab:某个属性信息 -->
<center><img src="/zh-cn/images/ProductManagement/list10.png" alt="img" style="zoom:100%;" /></center>

<!-- tab:产品关联设置截图 -->
<center><img src="/zh-cn/images/ProductManagement/list24.png" alt="img" style="zoom:100%;" /></center>


<!-- tab:工作逻辑示意图 -->
<center><img src="/zh-cn/images/ProductManagement/list22.png" alt="img" style="zoom:100%;" /></center>


<!-- tabs:end -->



### 创建产品属性

> 这里创建的产品属性是可以通用的，可同时给N个产品关联使用。
>
> OPS系统会预制一些常规通用的产品属性，你也可以根据自己的业务需求增加所需的。

1. **首先**进入产品属性，路径：系统后台->[产品管理](/zh-cn/ProductManagement)->[产品属性](/zh-cn/ProductManagement?id=产品属性)

2. **例如**添加一个**快递付费方式的**产品属性，表单说明见：[产品属性表单](/zh-cn/TopicAdditionalTable?id=产品属性表单)

<!-- tabs:start -->

<!-- tab:1.进入产品属性 -->
<center><img src="/zh-cn/images/ProductManagement/list9.png" alt="img" style="zoom:100%;" /></center>

<!-- tab:2.添加产品属性 -->
创建产品属性表单截图

<img src="/zh-cn/images/ProductManagement/list12.png" alt="img" style="zoom:100%;" />
<!-- tabs:end -->

### 设置产品属性

> 这里设置产品属性是指当属性中所需的项目，可以根据业务需求进行增加调整。

例如`快递付费方式`有多种，那就根据当前业务需求进行增加。

1.  找到[创建产品属性](/zh-cn/QuickPrint-SetProductAttributes?id=创建产品属性)这一步创建的产属性，点击`查看产品属性`
2. 在产品属性信息列表点击`添加`，如下图表单，表单说明见：[产品属性项目](/zh-cn/TopicAdditionalTable?id=产品属性项目)

<!-- tabs:start -->

<!-- tab:添加产品属性信息 -->
<center><img src="/zh-cn/images/ProductManagement/list11.png" alt="img" style="zoom:100%;" /></center>


<!-- tab:快递属性信息列表 -->
<center><img src="/zh-cn/images/ProductManagement/list10.png" alt="img" style="zoom:100%;" /></center>
<!-- tabs:end -->



### 结束语

> 已经了解与熟悉产品属性，那我们可以进行下一步学习：[从零发布一个产品](/zh-cn/TopicQuickPrint-AddNewProduct)

?> 提示：可以不着急创建太多产品属性，可以根据[自定义产品属](/zh-cn/QuickPrint-AddNewProduct?id=第三步：自定义属性)性业务时，根据需求进行创建。

!> 与生产无关的属性可自己调整与添加，与`生产相关属性`请于我们技术沟通调整。

**生产属性例如：**

- 单双面
- 设备机型
- 纸张尺寸
- ......

[前台属性排序小技巧](/zh-cn/Query?id=前台属性排序在哪里修改？)



<p align="right">Document creation time:2021-12-29   Update time:{docsify-updated} </p> 
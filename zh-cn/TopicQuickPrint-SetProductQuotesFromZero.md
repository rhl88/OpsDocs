## 从零设置产品报价

> 快印产品的报价可以DIY形式可多选各项工艺进行下单，让客户拥有细节可控选项根据需求定制化自己所需求的产品。

### 一、基础了解
>  到了这里说明已掌握从[设置一个产品属性](/zh-cn/TopicQuickPrint-SetProductAttributes)到[发布产品](/zh-cn/TopicQuickPrint-AddNewProduct)，那么我们继续把整个流程贯穿进行设置产品报价 。


产品的最终报价涉及到**报价表**和当前账户的**优惠分组**、**阶梯价格分组**。

接下来，我们就围绕这些进行了解和学习。

**产品报价相关截图**
<!-- tabs:start -->

<!-- tab:前台价格展示 -->
<center><img src="/zh-cn/images/Topic/list25.png" style="zoom:100%;" /></center>
<!-- tab:报价表后台展示 -->
<center><img src="/zh-cn/images/Cost-related/list10.png" style="zoom:100%;" /></center>
<!-- tab:阶梯价格后台展示 -->
<center><img src="/zh-cn/images/Cost-related/list13.png" style="zoom:100%;" /></center>
<!-- tab:优惠分组后台展示 -->
<center><img src="/zh-cn/images/Cost-related/list7.png" style="zoom:100%;" /></center>
<!-- tab:阶梯价格分组后台展示 -->
<center><img src="/zh-cn/images/Topic/list52.png" style="zoom:100%;" /></center>
<!-- tab:设置快印报价流程示意 -->
<center><img src="/zh-cn/images/Cost-related/list9.png" style="zoom:100%;" /></center>

<!-- tabs:end -->
### 1.报价表的组成
##### 什么是报价单？

> 是根据产品或者产品相关连的工艺及自定义**属性**进行关联**组合**制定的**定价体系**规则称之为**多维度**组合报价。

**举例：**根据需可以将 【颜色+纸张克重+单双面】产品工艺进行创建多维度组合成一个**报价单**。

<!-- tabs:start -->
<!-- tab:报价单截图 -->
<img src="/zh-cn/images/Cost-related/list11.png" alt="img" style="zoom:100%;" />
<!-- tab:多维度报价列表 -->
<img src="/zh-cn/images/Cost-related/list12.png" alt="img" style="zoom:100%;" />
<!-- tabs:end -->

##### 什么是报价表？

> 报价表是有大量的报价单而形成的。

<!-- tabs:start -->
<!-- tab:报价表逻辑 -->

<center>

```mermaid
graph TB
    1A(系统后台)
    1A-->1B(定价体系)
    1B-->1C(报价表)
    1C-->|报价单|1D(适配工艺)
    2A(前台下单)
    2A-->2B(选择产品)
    2B-->2C(选择工艺)
    2C-->|所选工艺|1D(适配工艺)
    3A(进行报价)
    1D-->|费用计算|3A
```

报价表费用计算功能示意</center>

<!-- tab:报价表截图 -->
<img src="/zh-cn/images/Cost-related/list10.png" alt="img" style="zoom:100%;" />
<!-- tabs:end -->

### 2.优惠分组
> 优惠分组是指可设置不同价格折扣组，可让更灵活的控制不同企业客户所享受的价格优惠。

举例：一些预存客户或者大客户在原有基础上进行打9折或者9.5折，那么就新建一个专属的原价上的折扣。
<!-- tabs:start -->

<!-- tab:优惠结算示意 -->

<center>

```mermaid
graph TB
    1(订单结算) --> 2(订单价格)
    2--> |检测所在组|2A(分组)
    2A --> 2B(所在组1)
    2A--> 2C(所在组2)
    2A--> 2D(所在组N)
    2E(最终折扣)
    2B-->|8折|2E
    2C-->|6折|2E
    2D-->|N折|2E
```

优惠分组结算逻辑示意</center>

<!-- tab:优惠后台展示 -->
<center><img src="/zh-cn/images/Cost-related/list7.png" style="zoom:100%;" /></center>

<!-- tabs:end -->

### 3.阶梯价格分组

> 阶梯价格分组可以将不同的企业客户进行不同的阶梯分组报价。

举例：

1. 阶梯价格有2个分组，价格分`组1` 的报价是1-99 每张1元。`分组2`的报价1-99份每张0.9元。
2. 有A,B,C,D四个客户，我们设置A,B客户为`分组1`、C,D客户为`分组2`，在同一个产品将执行不同的价格阶梯报价方式。
3. 如果当前用户没有特定分组，就会获取默认正常报价。

<!-- tabs:start -->
<!-- tab:阶梯价格分组结算示意 -->

<center>

```mermaid
graph TB
    1A(产品报价)-->2A
    1C-->|每张1元|1G
    1D-->|每张0.9元|1G
    2A(企业客户)
    2A-->2B(A)
    2A-->2C(B)
    1C(组1)
    2B-->1C
    2C-->1C
    2A-->2D(C)
    2A-->2E(D)
    1D(组2)
    XD(阶梯价格分组)
    XD-->1C
    XD-->1D
    2D-->1D
    2E-->1D
    1G(进行结算)
```

阶梯价格分组报价示意</center>


<!-- tab:阶梯价格分组后台展示 -->

<center><img src="/zh-cn/images/Topic/list52.png" style="zoom:100%;" /></center>

<!-- tabs:end -->

### 二、开始设置

##### 1、创建一个报价单

举例：机型颜色纸张关联报价

现在关联三个产品属性：`机型`、`颜色`、`纸张类型`

在机型 `4开`选择不同`颜色`所用`纸张类型`产生不同的报价


<!-- tabs:start -->
<!-- tab:关联逻辑示意图 -->
如果[产品自定义属性](/zh-cn/QuickPrint-SetProductAttributes)中如下设置：
<center><img src="/zh-cn/images/Topic/list1.gif" style="zoom:100%;" /></center>
<!-- tab:创建一个报价单 -->
不同颜色所对使用的纸张不同，需要选择当前产品属性为 `印刷设备机型`、`颜色`、`纸张类型` 如`报价属性关联示意图` 。
<center><img src="/zh-cn/images/Topic/list53.png" style="zoom:100%;" /></center>
<!-- tabs:end -->

##### 2、管理报价单

进入[管理报价表：设置关联价格规则](/zh-cn/PricingSystem?id=管理报价表：设置关联价格规则)，了解学习报价单相关设置。

##### 3、设置优惠分组

进入 [优惠定价分组管理设置](/zh-cn/PricingSystem?id=优惠定价分组)

##### 4、设置阶梯价格分组

进入 [阶梯价格分组管理设置](/zh-cn/PricingSystem?id=阶梯价格分组)

##### 5、了解 [默认价格库](/zh-cn/PricingSystem?id=默认价格库)

### 结束语
> 这节教程中的需要关联了解的地方比较多，需要重复阅读了解。

下一步：[从下单到生产管理指引](/zh-cn/TopicQuickPrint-FromAddOrderToProduction)

<p align="right">Document creation time:2021-12-29   Update time:{docsify-updated} </p> 
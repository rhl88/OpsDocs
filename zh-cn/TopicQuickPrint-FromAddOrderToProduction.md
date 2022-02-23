

## 从下单到生产管理指引

> 来到这一步就说明您已掌握了如何创建一个产品，下面讲述从前台下单到生产管理的一些操作。


### 前端订购过程

> 在下单上传文件时，需遵守`产品简介`中的规范要求，并阅读了解《[文件基本标准](/zh-cn/TopicBasicDocumentStandards?id=快印产品下单)》。

<!-- tabs:start -->

<!-- tab:1.登录前台账号 -->
需登录账号才可以进行下单，如没有账号可自行注册。

<img src="/zh-cn/images/Topic/list22.png" style="zoom:100%;" />

<!-- tab:2.选择产品类型 -->
<img src="/zh-cn/images/Topic/list23.png" style="zoom:100%;" />

<!-- tab:3.选择属性细节 -->
<img src="/zh-cn/images/Topic/list24.png" style="zoom:100%;" />

<!-- tab:4.查阅订购报价 -->
<img src="/zh-cn/images/Topic/list25.png" style="zoom:100%;" />

<!-- tab:5.加入购物车 -->
<img src="/zh-cn/images/Topic/list26.png" style="zoom:100%;" />

<!-- tab:6.提交订单 -->
<img src="/zh-cn/images/Topic/list27.png" style="zoom:100%;" />
<!-- tabs:end -->



### 后台管理工作
#### 订单查阅
> 订单查阅制作文件检查并确认制作文件


<!-- tabs:start -->
<!-- tab:1.制作订单 -->
进入顺序，系统后台->[订单管理](/zh-cn/OrderManagement?id=订单管理)->[制作订单](/zh-cn/OrderManagement?id=制作订单)；进入制作订单过程，点击`+`打开订单管理。
<img src="/zh-cn/images/Topic/list28.png" style="zoom:100%;" />

<!-- tab:2.编辑订单 -->
1. 先点击`①源文件`下载并检查或修改文件。
2. 如文件**有问题**需上传修正后确认订单文件，文件正常则无需上传（如没有下图中的`③`则把源文件确认没问题重新上传一下）。
3. 如客户前端选择属性错误可`⑤编辑属性`进行修改；
4. 如果该订单是含有多款订单需要点击`④手工拆单`，如果不需要或者设计好文件可以直接点击下一步，进行下一步操作；
   <img src="/zh-cn/images/Topic/list46.png" style="zoom:100%;" />

<!-- tab:3.下一步操作 -->
?> 在[订单管理](/zh-cn/OrderManagement)中[制作订单](/zh-cn/OrderManagement?id=制作订单)选择对应的订单点击`+`然后`编辑生产订单`再执行下一步操作。

   `正常步骤：审核->tflow处理(如需处理)->拼板->排产`

| 步骤      | 说明                                                         | 备注 |
| --------- | ------------------------------------------------------------ | ---- |
| 审核      | 可选经过下一步审核人员审核订单（`如不需要审核人员可跳过审核`） |      |
| 排产      | 可以直接发到排产状态（如直接到排产状态可跳去[排产](/zh-cn/QuickPrint-FromAddOrderToProduction?id=拼板查阅)下查阅文件并进行打印操作） |      |
| 拼板      | 当文件属于PDF并且已经设计好的文件可直接选择拼板处理，并跳到[查阅拼板](/zh-cn/QuickPrint-FromAddOrderToProduction?id=拼板查阅)结果界面 |      |
| Tflow处理 | 文件经过上一步操作后如未转PDF或者文件需要通过TFLOW进行拆单或者重新生成预览文件，点解通过`tflow处理`状态进入后台文件处理程序进行处理 |      |

<img src="/zh-cn/images/Topic/list47.png" style="zoom:100%;" />

**TFLOW处理**后去：动作说明

|  动作    |  说明  |  备注  |
| ---- | ---- | ---- |
| 审核  | TFLow处理后进入4.审核订单 |      |
|  排产 | TFLow处理后进入[订单排产](/zh-cn/QuickPrint-FromAddOrderToProduction?id=订单排产) |      |
|  拼版  | TFLow处理后进入[拼板查阅](/zh-cn/QuickPrint-FromAddOrderToProduction?id=拼板查阅) |      |
|  打印  | TFLow处理后进入 [打印管理](/zh-cn/QuickPrint-FromAddOrderToProduction?id=打印管理) |      |
|  上机  | TFLow处理后进入 发送到打印机 |      |

<img src="/zh-cn/images/Topic/list55.png" style="zoom:100%;" />

<!-- tab:4.审核订单 -->
> 在第3步时如选择TFLow处理时将跳过此步骤

1. 进入待审核管理
    <img src="/zh-cn/images/Topic/list49.png" style="zoom:100%;" />

2. 选择待审核订单 进行比对
    <img src="/zh-cn/images/Topic/list50.png" style="zoom:100%;" />

3. 进行比对并审核，`审核通过`进入拼版、`审核不通过`返回上一步

  如在此步骤看不到 `源文件制作模板` 、 `制作后文件` 可到第`2`步中的`文件信息`中点击`源文件`、`制作文件`  下载后进行比对后再进行审核。

  <img src="/zh-cn/images/Topic/list51.png" style="zoom:100%;" />
  <!-- tabs:end -->

#### 订单排产
> 进入订单排产，查看订单排产以及推单相关操作。

<!-- tabs:start -->

<!-- tab:1.进入排产 -->
勾选所需要（可多选）推送的订单点击`推单`按钮进行（推送到拼板）操作。
<img src="/zh-cn/images/Topic/list48.png" style="zoom:100%;" />

<!-- tab:2.推单操作 -->
| 操作           | 说明                                                         | 备注 |
| -------------- | ------------------------------------------------------------ | ---- |
| 推单           | 直接推送订单文件到拼板处理（含已拼板文件走一次推送流程）     |      |
| 推单并追加属性 | 可查看订单细节并重新选择机器类型（含已拼板文件走一次推送流程） |      |
| 手动拼板推送   | `预留设计中`                                                 |      |

<img src="/zh-cn/images/Topic/list32.png" style="zoom:100%;" />

<!-- tabs:end -->

#### 拼板查阅
> 查阅订单拼板结果并确认板文件，确认版文件后自动发送到打印管理。

<!-- tabs:start -->

<!-- tab:1.进入拼版结果 -->
点击下图中的`查看拼版结果`，即可进入拼版结果列表。
<img src="/zh-cn/images/Topic/list33.png" style="zoom:100%;" />


<!-- tab:2.查看拼板结果 -->
如果状态还在`拼版中`则需要等待，`一般几分钟`内就完成拼版(大文件除外)；如**长时间未更新状态**则及时联系我们协助处理。

`操作`按钮功能

| 操作         | 说明                                         | 备注 |
| ------------ | -------------------------------------------- | ---- |
| 回退         | 可撤销拼板操作返回推单界面重新推送到拼板处理 |      |
| 确认拼板     | 确认拼板后往下进入生产管理栏目进行打印管理   |      |
| 上传拼板文件 | 可手动重新上传一个拼板文件并重新选择制作信息 |      |

<img src="/zh-cn/images/Topic/list34.png" style="zoom:100%;" />


<!-- tab:3.订单拼板信息 -->
在第2步中订单的拼板信息，点击`版文件`**图标**可以在线预览文件，调用AI版文件编辑（`待完善功能`）；

`打印批次单`可配置打印机把批次订单信息打印出来（`待完善功能`）。

更新放数即可增加印张数（`可选`）

<img src="/zh-cn/images/Topic/list35.png" style="zoom:100%;" />
<!-- tabs:end -->

#### 打印管理
> 生产管理订单打印以及机器状态管理

<!-- tabs:start -->
<!-- tab:1.打印列表 -->
> 在打印管理界面可以查阅到已经完成拼板并确认可上机处理的订单状态

- 待处理模块：订单在等待确认上机打印状态或已上机等待印刷。
- 已处理模块：订单文件已经完成印刷结束整个订单制作印刷环节。

打印状态
- 待打印：已完成拼版等待打印。
- 移动中：文件移动中即将上机
- 已上机：已上机印刷中。
- 已印刷：已完成印刷。


<img src="/zh-cn/images/Topic/list36.png" style="zoom:100%;" />

<!-- tab:2.打印操作 -->
`操作`按钮功能

| 操作         | 说明                                         | 备注 |
| ------------ | -------------------------------------------- | ---- |
| 打印| 文件JDF自动移动到机器使得文件在打印机预打印状态 |(`待打印`状态) |
| 补印|重新推送打印（`开发设计中`）|(`已打印`状态) |
| 重推     | 文件自动打印重新推送一次   |(`移动中`状态)|
| 编辑 | 编辑当前打印（`开发设计中`） |      |
| 删除 | 删除打印管理订单文件，删除已印刷文件(`已打印`状态) |      |

<img src="/zh-cn/images/Topic/list37.png" style="zoom:100%;" />

<!-- tabs:end -->


### 串联整个过程

<!-- tabs:start -->
<!-- tab:整个流程示意 -->

<img src="\zh-cn\images\Topic\list54.png" style="zoom:100%;" />
<!-- tabs:end -->

<p align="right">Document creation time:2021-12-31   Update time:{docsify-updated} </p> 
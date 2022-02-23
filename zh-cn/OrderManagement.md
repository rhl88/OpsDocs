# 订单管理

> 下单订单管理系统基本操作使用文档。

## 订单列表

汇集前台客户下单统一管理以及处理。

<!-- tabs:start -->

<!-- tab:订单列表 -->
> 产品订单列表，可查看订单信息以及快速订单管理。

操作功能说明

| 功能         | 说明             | 备注                              |
| ------------ | ---------------- | --------------------------------- |
| 订单详情     | 查看订单详细信息 | 功能截图：见上方切换Tab`订单详情` |
| 审核/重传    | | `待完善`                          |
| 删除订单     | 将此订单彻底删除 |                                   |
| 修改收货地址 |                  | `待完善`                          |
| 批量打单     |                  | `待完善`                          |
| 取消订单     |                  | `待完善`                          |
| 发货【顺丰】 |                  | `待完善`                          |

<img src="\zh-cn\images\OrderManagement\list01.png" style="zoom:80%;" />


<!-- tab: 订单详情 -->
> 当前订单详细信息以及订单状态

<img src="\zh-cn\images\OrderManagement\list02.png" style="zoom:80%;" />

<!-- tab:产品单信息 -->

>  在产品列表中双击想要查看的订单即可显示如下产品信息。

<img src="\zh-cn\images\OrderManagement\list04.png" style="zoom:80%;" />
<!-- tabs:end -->

## 生产单列表
> 进入TFLow自动拼版生产管理列表。
<!-- tabs:start -->

<!-- tab: 生产单列表 -->

操作功能说明

| 功能         | 说明             | 备注                              |
| ------------ | ---------------- | --------------------------------- |
| 订单详情     | 查看订单详细信息 | 功能截图：[订单列表](/zh-cn/OrderManagement?id=订单列表)切换Tab`订单详情` |
| 查看文件    |  查看待处理文件  | 功能截图：见上方切换Tab`查看文件` |
| 生产跟踪     | 生产[流程工序](/zh-cn/ProductionManagement?id=生产工序列表)跟踪,可以看到每步工序操作人员 |                                   |
| 暂停&恢复生产 |  暂停恢复生产程序  |                       |
| 下载生产文件     | 下载拼版后的成品待印刷文件   |                     |
| 整本报片     |重新提交整本    |      |

<img src="\zh-cn\images\OrderManagement\list05.png" style="zoom:80%;" />


<!-- tab: 查看文件 -->
> 图片文件会直接显示缩略图，主要应用于`影像产品`。


<img src="\zh-cn\images\OrderManagement\list06.png" style="zoom:80%;" />


<!-- tabs:end -->

## 待确认订单

> 等待审核确认的订单列表

<img src="\zh-cn\images\OrderManagement\list07.png" style="zoom:80%;" />

## 制作订单

<!-- tabs:start -->

<!-- tab: 制作订单列表 -->
> 进入制作订单过程，点击`+`打开订单管理。
> 

<img src="/zh-cn/images/Topic/list28.png" style="zoom:80%;" />

<!-- tab: 编辑生产单 -->

1. 先点击`源文件`下载并检查或修改文件。
2. 如文件**有问题**需上传修正后确认订单文件，文件正常则无需上传。
3. 如客户前端选择属性错误可`编辑属性`进行修改；
4. 如果该订单是含有多款订单需要点击`手工拆单`，如果不需要或者设计好文件可以直接点击下一步；将由TFLow自动处理。

<img src="/zh-cn/images/Topic/list46.png" style="zoom:100%;" />

<!-- tab: 下一步操作 -->
?> 在**订单管理**中**制作订单**选择对应的订单点击`+`然后`编辑生产订单`再执行下一步操作时。

`正常步骤：审核->tflow处理(如需处理)->拼板->排产`

| 步骤      | 说明                                                         | 备注 |
| --------- | ------------------------------------------------------------ | ---- |
| 审核      | 可选经过下一步审核人员审核订单（`如不需要审核人员可跳过审核`） |      |
| 排产      | 可以直接发到排产状态（如直接到排产状态可跳去[排产](/zh-cn/TopicProductionOperationProcess?id=拼板查阅)下查阅文件并进行打印操作） |      |
| 拼板      | 当文件属于PDF并且已经设计好的文件可直接选择拼板处理，并跳到[查阅拼板](/zh-cn/OrderManagement?id=拼板查阅)结果界面 |      |
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

<!-- tabs:end -->

## 订单排产

> 进入订单排产，查看订单排产以及推单相关操作。

<!-- tabs:start -->
<!-- tab: 排产列表 -->
勾选所需要（可多选）推送的订单点击`推单`按钮进行（推送到拼板）操作。
<img src="/zh-cn/images/Topic/list31.png" style="zoom:100%;" />

<!-- tab: 推单操作 -->
| 操作           | 说明                                                         | 备注 |
| -------------- | ------------------------------------------------------------ | ---- |
| 推单           | 直接推送订单文件到拼板处理（含已拼板文件走一次推送流程）     |      |
| 推单并追加属性 | 可查看订单细节并重新选择机器类型（含已拼板文件走一次推送流程） |      |
| 手动拼板推送   | 预留设计中                                                   |      |

<img src="/zh-cn/images/Topic/list32.png" style="zoom:100%;" />

<!-- tabs:end -->


#### 拼板查阅
> 查阅订单拼板结果并确认板文件，确认版文件后自动发送到打印管理。

<!-- tabs:start -->
<!-- tab: 进入拼版结果 -->
在[订单排产](/zh-cn/OrderManagement?id=订单排产)点击下图中的`查看拼版结果`，即可进入拼版结果列表。
<img src="/zh-cn/images/Topic/list33.png" style="zoom:100%;" />
<!-- tab: 查看拼板结果 -->
`操作`按钮功能

| 操作         | 说明                                         | 备注 |
| ------------ | -------------------------------------------- | ---- |
| 回退         | 可撤销拼板操作返回推单界面重新推送到拼板处理 |      |
| 确认拼板     | 确认拼板后往下进入生产管理栏目进行打印管理   |      |
| 上传拼板文件 | 可手动重新上传一个拼板文件并重新选择制作信息 |      |

<img src="/zh-cn/images/Topic/list34.png" style="zoom:100%;" />

<!-- tab: 订单拼板信息 -->

订单的拼板信息，版文件，点击版文件可以在线预览文件，调用AI版文件编辑（`待完善功能`）；

`打印批次单`可配置打印机把批次订单信息打印出来（`待完善功能`）。

更新放数即可增加印张数（`可选`）

<img src="/zh-cn/images/Topic/list35.png" style="zoom:100%;" />
<!-- tabs:end -->


<p align="right">Document creation time:2021-12-22   Update time:{docsify-updated} </p> 
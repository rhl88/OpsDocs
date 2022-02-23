# 标准字段
> 在OPS系统功能处理中规范标准使用字段。



**字段导航：**

| [后道工序](/zh-cn/StandardFields?id=后道工序) | [印刷](/zh-cn/StandardFields?id=印刷) | [纸张](/zh-cn/StandardFields?id=纸张) | [拼版](/zh-cn/StandardFields?id=拼版) | [脚注](/zh-cn/StandardFields?id=脚注) | [数量](/zh-cn/StandardFields?id=数量) | [尺寸](/zh-cn/StandardFields?id=尺寸) |
| --------------------------------------------- | ------------------------------------- | ------------------------------------- | ------------------------------------- | ------------------------------------- | ------------------------------------- | ------------------------------------- |

## 字段使用

### 在TFLow中使用
在**Script**中引入OPS
``` csharp
//引入OPS
var ops = instance.Ops;
//使用OPSLabel字段
//赋值
int runLength = ops.runLength; 
//直接使用
if(ops.runLength>0){

}
```

#### 数值使用

类型：float

浮点类型
``` csharp
//引入OPS
var ops = instance.Ops;

//赋值使用
float Weight = ops.substrateWeight; 
float size = Weight*2.5f;

//直接使用
size = ops.substrateWeight*2.5f;
```
类型：int

整数类型
``` csharp
//引入OPS
var ops = instance.Ops;

//赋值使用
int placed = ops.placed; 
int amount = placed*2;

//直接使用
amount = ops.placed*2;
```

#### 字符串
类型：string
``` csharp
//引入OPS
var ops = instance.Ops;

//赋值使用
string Address = ops.deliveryAddress; 
string amount = placed*2;

//直接使用
Address = ops.deliveryAddress;
```

#### 布尔值
类型：bool
``` csharp
//引入OPS
var ops = instance.Ops;

//赋值使用
bool DoubleSide = ops.isDoubleSide; 
if(DoubleSide==true){ //双面

}

//直接使用
if(ops.isDoubleSide==true){ //双面

}
```

#### itemLabel
类型：Label名
``` csharp
//引入OPS
var ops = instance.Ops;

//方法1 推荐
if(ops.digitalPrinter==DigitalPrinter.indigo7900){ //indigo7900打印机

}

//方法2 不推荐
if(ops.digitalPrinter=="indigo7900"){ //indigo7900

}
```
## 字段表



### 后道工序
| Label           | itemLabel              | 类型           | 标准名称         | 别名                   | 描述 |
| --------------- | ---------------------- | -------------- | ---------------- | ---------------------- | ---- |
| laminationType  |                        | LaminationType | 覆膜类型         | 后道增效，覆膜         |      |
|                 | matte                  |                | 覆哑膜           |                        |      |
|                 | glossy                 |                | 覆光膜           |                        |      |
| bindingType     |                        | BindingType    | 装订方式         |                        |      |
|                 | saddleStich            |                | 骑马钉           |                        |      |
|                 | perfectBind            |                | 无线胶装         |                        |      |
| cutType         |                        | CutType        | 切割方式         |                        |      |
|                 | singleCut              |                | 单刀             |                        |      |
|                 | doubleCut              |                | 双刀             |                        |      |
|                 | singleCutTBdoubleCutLR |                | 上下单刀左右双刀 |                        |      |
|                 | doubleCutTBsingleCutLR |                | 上下双刀左右单刀 |                        |      |
|                 | kissCut                |                | 划刀             | 半透                   |      |
|                 | dieCut                 |                | 割刀（割断）     | 割样，膜切，模切，全透 |      |
|                 | crease                 |                | 压痕             |                        |      |
| foldingPatterns |                        | string         | 折手样式         | 折页，折手             |      |

### 印刷
| Label          | itemLabel          | 类型           | 标准名称   | 别名     | 描述 |
| -------------- | ------------------ | -------------- | ---------- | -------- | ---- |
| digitalPrinter |                    | DigitalPrinter | 数字印刷机 |          |      |
|                | indigo7900         |                |            |          |      |
|                | indigo5600         |                |            |          |      |
|                | indigo12000        |                |            |          |      |
| offsetPress    |                    | string         | 传统印刷机 |          |      |
| printColorMode |                    | PrintColorMode | 颜色       | 印刷颜色 |      |
|                | fourColorPrint     |                | 4色打印    |          |      |
|                | sixColorPrint      |                | 6色打印    |          |      |
|                | blackAndWhitePrint |                | 黑白打印   |          |      |

### 纸张
| Label           | itemLabel   | 类型     | 标准名称   | 别名     | 描述                     |
| --------------- | ----------- | -------- | ---------- | -------- | ------------------------ |
| pageType        |             | PageType | 纸张类型   |          |                          |
|                 | mattePaper  |          | 哑粉纸     |          |                          |
|                 | glossyPaper |          | 铜版纸     |          |                          |
| substrateWeight |             | float    | 承印物克重 | 纸张厚度 | 类型与克重分开写时用     |
| substrate       |             | string   | 承印物名称 | 纸张名称 | 类型与克重一起写的时候用 |

### 拼版
| Label          | itemLabel  | 类型           | 标准名称           | 别名     | 描述 |
| -------------- | ---------- | -------------- | ------------------ | -------- | ---- |
| bleed          |            | float          | 出血               | 四周出血 |      |
| bleedBottom    |            | float          | 下出血             |          |      |
| bleedTop       |            | float          | 上出血             |          |      |
| bleedLeft      |            | float          | 左出血             |          |      |
| bleedRight     |            | float          | 右出血             |          |      |
| isDoubleSide   |            | bool           | 单双面             |          |      |
|                | true       |                | 双面               |          |      |
|                | false      |                | 单面               |          |      |
| filePageNum    |            | int            | 文件页数           |          |      |
| fileSpine      |            | float          | 书脊               |          |      |
| hasDieLine     |            | bool           | 是否含专色刀线     |          |      |
|                | true       |                | 是                 |          |      |
|                | false      |                | 否                 |          |      |
| rotation       |            | Rotation       | 旋转方式           |          |      |
|                | any        | string         | 自由旋转           |          |      |
|                | none       | string         | 不选转保持原方向   |          |      |
| grainDirection |            | GrainDirection | 文件方向与纸纹方向 |          |      |
|                | vertical   |                | 垂直               |          |      |
|                | horizontal |                | 水平               |          |      |
|                | none       |                | 无                 |          |      |
| isJobGang      |            |                | 是否混拼           |          |      |
|                | true       |                | 混拼               |          |      |
|                | false      |                | 专版               |          |      |
| isNeedImpose   |            | bool           | 是否拼版           |          |      |
|                | true       |                | 需要拼版           |          |      |
|                | false      |                | 不需要拼版         |          |      |

### 脚注
| Label            | itemLabel | 类型   | 标准名称 | 别名                       | 描述 |
| ---------------- | --------- | ------ | -------- | -------------------------- | ---- |
| deliveryAddress  |           | string | 送货地址 | 收货地址，地址，收件人地址 |      |
| remark           |           | string | 备注     |                            |      |
| contractNumber   |           | string | 合同号码 |                            |      |
| salesOrderNumber |           | string | 销售单号 |                            |      |
| deliveryDate     |           | string | 送货日期 |                            |      |

### 数量
| Label         | itemLabel | 类型       | 标准名称                       | 别名      | 描述                                                   |
| ------------- | --------- | ---------- | ------------------------------ | --------- | ------------------------------------------------------ |
| orderQuantity |           | int        | 采购数量                       |           |                                                        |
| runLength     |           | int        | 印刷张数                       |           | 印刷张数（车头数）                                     |
| placed        |           | int        | 放置个数                       | 拼数,片数 | 每版放置的个数                                         |
| isOrdQtySumUp |           | bool       | 同一文件拆款后订购数量是否累计 |           | 同一文件，拆多款后，订购数量是否累计，用于优惠价格计算 |
|               | true      |            | 是                             |           |                                                        |
|               | false     |            | 否                             |           |                                                        |
| getQtyFrom    |           | GetQtyFrom | 数量获取方式                   |           |                                                        |
|               | fromWeb   |            | 提交工具输入                   |           |                                                        |
|               | fromFile  |            | 来自文件(标签、画板)           |           |                                                        |

### 尺寸
| Label                        | itemLabel | 类型  | 标准名称              | 别名                   | 描述                                         |
| ---------------------------- | --------- | ----- | --------------------- | ---------------------- | -------------------------------------------- |
| unfoldFileWidthxFileHeight   |           | float | 册子展开尺寸(含出血） | 内页展开尺寸           | 册子展开后的内页尺寸                         |
| fileTrimWidthxFileTrimHeight |           | float | 净尺寸（裁切尺寸）    |                        |                                              |
| fileWidthxFileHeight         |           | float | 尺寸(含出血）         | 单页尺寸,画册折叠尺寸, | 折叠时的尺寸                                 |
| fileTrimHeight               |           | float | 文件净高度            |                        |                                              |
| fileTrimWidth                |           | float | 文件净宽度            |                        |                                              |
| fileHeight                   |           | float | 文件宽度（含出血）    | 册子高MM               | 文件宽度（含出血）                           |
| fileWidth                    |           | float | 文件高度（含出血）    | 册子宽MM               | 文件高度（含出血）                           |
| dynamicPrintMaxWidth         |           | float | 最大动态尺寸宽        | 最大宽度               |                                              |
| dynamicPrintMinWidth         |           | float | 最小动态尺寸宽        | 最小宽度               |                                              |
| dynamicPrintMinHeight        |           | float | 最小动态尺寸高        | 最大高度               |                                              |
| dynamicPrintMaxHeight        |           | float | 最大动态尺寸高        | 最小高度               |                                              |
| printMarginTop               |           | float | 纸张上边距            |                        | 印刷机上边空白                               |
| printMarginBottom            |           | float | 纸张下边距            |                        | 印刷机下边空白                               |
| printMarginRight             |           | float | 纸张右边距            |                        | 印刷机右边空白                               |
| printMarginLeft              |           | float | 纸张左边距            |                        | 印刷机左边空白                               |
| printWidth                   |           | float | 打印宽度              | 纸张宽度               | 印刷机宽度（含边空白，减去空白才是打印范围） |
| printHeight                  |           | float | 打印高度              | 纸张高度               | 印刷机高度（含边空白，减去空白才是打印范围） |
| printWidthxPrintHeight       |           | float | 拼板尺寸              |                        | 印刷机宽x高（含边空白）                      |



## 待定Label

新增字段待定Label

### 待定拼版

| Label           | itemLabel   | 类型  | 标准名称   | 别名     | 描述                               |
| --------------- | ----------- | ----- | ---------- | -------- | ---------------------------------- |
|                 |             |       | 出血方式   | 出血类型 |                                    |
|                 | bleed       |       | 四周出血   |          |                                    |
|                 |             |       | 上下出血   |          |                                    |
|                 |             |       | 左右出血   |          |                                    |
|                 | bleedBottom |       | 下出血     |          |                                    |
|                 | bleedTop    |       | 上出血     |          |                                    |
|                 | bleedLeft   |       | 左出血     |          |                                    |
|                 | bleedRight  |       | 右出血     |          |                                    |
| substrateWeight |             |       | 承印物克重 |          | 已整理常见克重                     |
|                 | 28          | float | 28         |          |                                    |
|                 | 30          | float | 30         |          |                                    |
|                 | 32          | float | 32         |          |                                    |
|                 | 35          | float | 35         |          |                                    |
|                 | 36          | float | 36         |          |                                    |
|                 | 48          | float | 48         |          |                                    |
|                 | 48.8        | float | 48.8       |          |                                    |
|                 | 58          | float | 58         |          |                                    |
|                 | 60          | float | 60         |          |                                    |
|                 | 64          | float | 64         |          |                                    |
|                 | 65          | float | 65         |          |                                    |
|                 | 70          | float | 70         |          |                                    |
|                 | 80          | float | 80         |          |                                    |
|                 | 90          | float | 90         |          |                                    |
|                 | 100         | float | 100        |          |                                    |
|                 | 105         | float | 105        |          |                                    |
|                 | 115         | float | 115        |          |                                    |
|                 | 120         | float | 120        |          |                                    |
|                 | 125         | float | 125        |          |                                    |
|                 | 128         | float | 128        |          |                                    |
|                 | 130         | float | 130        |          |                                    |
|                 | 150         | float | 150        |          |                                    |
|                 | 157         | float | 157        |          |                                    |
|                 | 160         | float | 160        |          |                                    |
|                 | 170         | float | 170        |          |                                    |
|                 | 180         | float | 180        |          |                                    |
|                 | 190         | float | 190        |          |                                    |
|                 | 200         | float | 200        |          |                                    |
|                 | 210         | float | 210        |          |                                    |
|                 | 230         | float | 230        |          |                                    |
|                 | 250         | float | 250        |          |                                    |
|                 | 300         | float | 300        |          |                                    |
|                 | 350         | float | 350        |          |                                    |
|                 | 400         | float | 400        |          |                                    |
|                 | 450         | float | 450        |          |                                    |
|                 | 500         | float | 500        |          |                                    |
|                 | 550         | float | 550        |          |                                    |
|                 | 600         | float | 600        |          |                                    |
|                 | 650         | float | 650        |          |                                    |
|                 | 700         | float | 700        |          |                                    |
| substrateWeight |             |       | 承印物名称 |          | 还有其它纸张同步`pageType`纸张类型 |
|                 | mattePaper  |       | 哑粉纸     |          |                                    |
|                 | glossyPaper |       | 铜版纸     |          |                                    |




### 待定尺寸

| Label | itemLabel | 类型   | 标准名称           | 别名     | 描述 |
| ----- | --------- | ------ | ------------------ | -------- | ---- |
|       |           |        |                    | 成品尺寸 |      |
|       | custom    | string | 自定义             |          |      |
|       | 740x510   | string | B2尺寸(740x510)    |          |      |
|       | 210x285   | string | 大度16开 (210x285) |          |      |
|       | 420x285   | string | 大度8开 (420x285)  |          |      |
|       | 420x580   | string | 大度4开 (420x580)  |          |      |
|       | 210x140   | string | 大度32开 (210x140) |          |      |
|       | 210x297   | string | A4尺寸(210x297)    |          |      |
|       | 185x260   | string | 正度16开 (185x260) |          |      |
|       | 260x380   | string | 正度8开 (260x380)  |          |      |
|       | 530x380   | string | 正度4开 (530x380)  |          |      |
|       | 185x125   | string | 正度32开 (185x125) |          |      |

### 待定印刷

| Label           | itemLabel   | 类型  | 标准名称   | 别名     | 描述                               |
| --------------- | ----------- | ----- | ---------- | -------- | ---------------------------------- |
| printColorMode |             |       | 颜色       | 印刷颜色 |                                    |
|                 | none        |       | 无         |          |                                    |

### 待定后道工序

| Label           | itemLabel   | 类型  | 标准名称   | 别名     | 描述                               |
| --------------- | ----------- | ----- | ---------- | -------- | ---------------------------------- |
| craft |  |  | 后道工艺 |  |  |
| creaseAmount |  |  | 压痕数量 |  |  |
| creaseType |  |  | 压痕方式 |  |  |
|  |  |  | 压痕不折 |  |  |
|  |  |  | 压痕折 |  |  |
| laminationType |           |  | 覆膜类型 | 覆膜 |      |
|                      | none |        | 无 |      |      |
| foldingPatterns |           |        | 折手样式     | 折页，折手 |      |
|                      | halfFold |        | 对折 |      |      |
|                      | threeFoldOrgan |        | 三折页风琴折 |      |      |
|                      | threeFoldWrap |        | 三折页包心折 |      |      |
|                      | fourFoldOrgan |        | 四折页风琴折 |      |      |
|                      | fourFoldCloseDoor |        | 四折页关门折 |      |      |
|                      | none |        | 无 |      |      |
|                      |           |        |                    |      |      |


### 待定其它

| Label           | itemLabel   | 类型  | 标准名称   | 别名     | 描述                               |
| --------------- | ----------- | ----- | ---------- | -------- | ---------------------------------- |
| uploadFile |           |        | 上传文件 |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |
|                      |           |        |                    |      |      |

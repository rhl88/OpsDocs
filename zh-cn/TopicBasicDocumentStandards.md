# 文件基本标准

> OPS系统前端文件提交标准化指引，下单时上传文件的基本标准说明，规范此基础标准可避免不必要的麻烦和错误。

## 快印产品下单

### 提交下单

产品下单文件提交含有两种方式，提交方式有`输入数量`以及`文件内写明`两种，如下图。

<!-- tabs:start -->

#### **输入数量**

<center>
<img src="\zh-cn\images\Topic\list02.png" style="zoom:100%;" />

单款输入数量
</center>

-------

<center>
<img src="\zh-cn\images\Topic\list04.png" style="zoom:100%;" />

多款相同输入数量
</center>

#### **文件内写明**

<center>
<img src="\zh-cn\images\Topic\list03.png" style="zoom:100%;" />

多款不同文件内写明
</center>

<!-- tabs:end -->

### PDF文件

1. 当文件属于`单款`，文件只需要填写数量。
2.  当文件属于`多款相同数量`时，我们会根据提交所选择的单双面自动按照单双面拆分出款数。
3.  当文件属于`多款不同数量`情况，总数量为文件内需要在书签内注明，当`单面`PDF时书签数量必须与P数相同，当`双面`时书签数必须时P数的1/2（如下图）。

<!-- tabs:start -->



#### **单面数量书签设置**

<center>
<img src="\zh-cn\images\Topic\list05.png" style="zoom:60%;" />

单面PDF签数量必须与P数相同
</center>



#### **双面数量书签设置**

<center>
<img src="\zh-cn\images\Topic\list06.png" style="zoom:60%;" />

当双面时书签数必须时P数的1/2
</center>



<!-- tabs:end -->

#### 刀线文件设置

若文件含有刀线，刀线颜色名称必须是`cut`
<center>
<img src="\zh-cn\images\Topic\list17.png" style="zoom:60%;" />

刀线文件设置示意
</center>

### AI文件

AI文件基本标准，设计文件必须放置在画板位置，建议最优方式时设计文件与画板大小相同。

1. 当`单款`、`多款相同数量`方式根据提交时输入数量即AI文件转pdf即可。

2. 当`多款不同数量`情况AI文件根据文件写明方式读取数量，设置画板的数量为每个单文件的份数。

举例：

设计文件有9个，单独设置9个画板承载，并在每个画板上设置名字为数量（如下图）。

<center>
<img src="\zh-cn\images\Topic\list07.png" style="zoom:60%;" />

AI文件份数示意图
</center>




### Cdr文件

Cdr文件处理说明
1.	处理逻辑：按照对象搜索，顺序从大到小，从左到右，从上到下，
2.	搜索对象：框体，组合，图片等
3.	过滤对象：框外备注信息（转曲不会被过滤），辅助线，
4.	群组内容：在文件设计中建议进来把设计内容进行群组。

系统对CDR转PDF，会自动提取文件；提交订单选择`多款不同数量`时，根据`页数`建立`画布`并在画布上输入单P文件的数量（如下图）。

<center>
<img src="\zh-cn\images\Topic\list08.png" style="zoom:60%;" />

画布命名示意图
</center>


**示例：名片**
<!-- tabs:start -->
#### **名片CDR文件**

<center>
<img src="\zh-cn\images\Topic\list09.png" style="zoom:100%;" />

名片CDR文件
</center>

#### **名片PDF结果**

<center>
<img src="\zh-cn\images\Topic\list10.png" style="zoom:60%;" />

名片PDF结果
</center>

<!-- tabs:end -->

**示例：单页**
<!-- tabs:start -->
#### **单页CDR文件**

<center>
<img src="\zh-cn\images\Topic\list11.png" style="zoom:100%;" />


单页CDR文件
</center>

#### **单页PDF结果**

<center>
<img src="\zh-cn\images\Topic\list12.png" style="zoom:60%;" />

单页PDF结果
</center>

<!-- tabs:end -->



**示例：多页**
<!-- tabs:start -->
#### **多页CDR文件**

<center>
<img src="\zh-cn\images\Topic\list13.png" style="zoom:100%;" />

多页CDR文件
</center>

#### **多页PDF结果**

<center>
<img src="\zh-cn\images\Topic\list14.png" style="zoom:60%;" />

多页PDF结果
</center>

<!-- tabs:end -->

#### 错误示范

**示范：错误1**
<!-- tabs:start -->
#### **错误1：CDR文件**

<center>
<img src="\zh-cn\images\Topic\list15.png" style="zoom:100%;" />

错误1 - CDR文件
</center>

#### **错误1：PDF结果**

<center>
<img src="\zh-cn\images\Topic\list16.png" style="zoom:60%;" />

错误1 - PDF结果
</center>

<!-- tabs:end -->

**示范：错误2**

1. 这里文字备注信息过滤成功
2. 右边方框视为内容对象导出

<center>
<img src="\zh-cn\images\Topic\list18.png" style="zoom:60%;" />

错误2 - 错误截图
</center>

**示范：错误3**
1. 组合式页面，不同内容是分开的。
2. 这种情况下，需要页面对象进行“组合”操作，或者用一个矩形框铺底，以最大框搜索原则。
3. 根据最大框搜索原则，底图会被提取出来。

<!-- tabs:start -->
#### **错误3：CDR文件**

<center>
<img src="\zh-cn\images\Topic\list19.png" style="zoom:100%;" />

错误3 - CDR文件
</center>

#### **错误3：PDF结果**

<center>
<img src="\zh-cn\images\Topic\list20.png" style="zoom:60%;" />

错误3 - PDF结果
</center>

<!-- tabs:end -->

### 文件输出目录示范
> 根据工程师对接设置不同而不同。

文件将根据四开，八开自动发送JDF以及文件地址刀相应机器，其他机型以及半刀或全刀文件根据以下目录结构输出到硬盘相应位置。
<center>
<img src="\zh-cn\images\Topic\list21.png" />

文件输出目录示范
</center>

------

## 影像产品下单

> 整理中

## 上传文件格式

目前系统支持格式如下表，根据不同类的产品要求不同

| 类型     | 格式 | 说明 | 备注   |
| -------- | ---- | ---- | ------ |
| 图片格式 |      |      |        |
|          | jpg  |      |        |
|          | jpeg |      |        |
|          | png  |      |        |
|          | tif  |      |        |
| 文档格式 |      |      |        |
|          | pdf  |      | `推荐` |
|          | doc  |      |        |
|          | docx |      |        |
|          | ppt  |      |        |
|          | pptx |      |        |
| 设计文件 |      |      |        |
|          | psd  |      |        |
|          | ai   |      |        |
|          | cdr  |      |        |
|          | indd |      |        |



## 文件基础标准

- 图片文件

  多个图片文件时宽高应保持一致，方便排版。

- pdf文件
  1. 每页尺寸与方向尽量保持一致，以免自动排版时处理出错。
  2. 若文件含有刀线，刀线颜色名称必须是cut
- 设计文件
  - pdf
  - ai
  - cdr
  - indd


- doc、docx
- ppt、pptx







<p align="right">Document creation time:2021-12-21   Update time:{docsify-updated} </p> 
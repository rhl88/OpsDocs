## 文档阅读指引

### 注解说明
> 一些名词、功能使用、描述或行业用语会在对应的字词中增加链接。

**例如：**

[DSS](/zh-cn/StartGuideMustRead?id=dss)套筒式技术为柔性印刷注入新活力。

在包装或装饰性印刷品中，常遇到一些花样设计满版重覆一致，又可随意裁切下来，而两端对接看不出接缝的要求，这在单色印刷机上，不论胶印或柔印，都是难以办到的。在卷筒式印刷机上虽能办到，但如果用单块式印版装到印版滚筒上去印刷，要做到印品看不出接缝，也同样是一件很困难的事。

单色如此，彩色就更困难。



###### DSS

DDS是指：(Digital Seamless Sleeves) 数字化无接缝套筒式印版。

### 图例说明

#### 展现形式

<!-- tabs:start -->

<!-- tab:连线说明 -->

| 形式     | 说明                                          | 图示                                                         |
| -------- | --------------------------------------------- | ------------------------------------------------------------ |
| 普通连线 | 下级或分类 `例如：客户种类、产品分类`         | <img src="\zh-cn\images\MustRead\014.png" alt="image" style="zoom:100%;" /> |
| 普通箭头 | 常规走向 `例如：产品管理->产品列表`           | <img src="\zh-cn\images\MustRead\015.png" alt="image" style="zoom:100%;" /> |
| 加粗连线 | 特别下级与分类 `重要或提示`                   | <img src="\zh-cn\images\MustRead\016.png" alt="image" style="zoom:100%;" /> |
| 加粗箭头 | 特别走向 `重要或提示`                         | <img src="\zh-cn\images\MustRead\017.png" alt="image" style="zoom:100%;" /> |
| 虚线连线 | **设想或假设**的下级或分类 `例如：假如、举例` | <img src="\zh-cn\images\MustRead\018.png" alt="image" style="zoom:100%;" /> |
| 虚线箭头 | **设想或假设**的走向                          | <img src="\zh-cn\images\MustRead\019.png" alt="image" style="zoom:100%;" /> |


<!-- tab:形状说明 -->

| 形状           | 功能说明                                                     | 形状图示                                                     | 示范                                                      |
| -------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | --------------------------------------------------------- |
| 直角矩形       | 菜单位置 `例如：产品管理->产品列表`                          | <img src="\zh-cn\images\MustRead\001.png" style="zoom:100%;" /> | [功能路径](/zh-cn/StartGuideMustRead?id=功能路径)         |
| 圆角矩形       | 功能按钮 `例如：添加、删除、编辑、操作`                      | <img src="\zh-cn\images\MustRead\002.png" style="zoom:100%;" /> | [功能操作](/zh-cn/StartGuideMustRead?id=功能操作)         |
| 体育场形       | 操作按钮 `例如：提交、确定`                                  | <img src="\zh-cn\images\MustRead\003.png" style="zoom:100%;" /> | [功能按钮](/zh-cn/StartGuideMustRead?id=功能按钮)         |
| 长灯光矩形     | 可选列表  `例如：操作功能中的 修改、删除等`                  | <img src="\zh-cn\images\MustRead\004.png" style="zoom:100%;" /> | [图例串联示范](/zh-cn/StartGuideMustRead?id=图例串联示范) |
| 圆柱体形       | 平台入口 `例如：OPS系统、TFLow系统、API接口`                 | <img src="\zh-cn\images\MustRead\005.png" style="zoom:100%;" /> | 同上                                                      |
| 正圆形         | 开始入口 `例如：系统后台、思路开始`                          | <img src="\zh-cn\images\MustRead\006.png" style="zoom:100%;" /> | 同上                                                      |
| 菱形           | 数据列表 `例如：子菜单、客户级别` 配合`标签形、长灯光矩形`使用较多 | <img src="\zh-cn\images\MustRead\008.png" style="zoom:100%;" /> | 同上                                                      |
| 标签形         | 单条数据 `例如：产品xxx、订单xxx`                            | <img src="\zh-cn\images\MustRead\007.png" style="zoom:100%;" /> | 同上                                                      |
| 六角形         | 信息汇总 `例如：客户A和客户B都 属于VIP3客户` 与**菱形**功能相反 | <img src="\zh-cn\images\MustRead\009.png" style="zoom:100%;" /> | [价格组](/zh-cn/PricingSystem?id=报价示例)                |
| 平行四边形     |                                                              | <img src="\zh-cn\images\MustRead\010.png" style="zoom:100%;" /> |                                                           |
| 反向平行四边形 |                                                              | <img src="\zh-cn\images\MustRead\011.png" style="zoom:100%;" /> |                                                           |
| 梯形           |                                                              | <img src="\zh-cn\images\MustRead\012.png" style="zoom:100%;" /> |                                                           |
| 倒梯形         |                                                              | <img src="\zh-cn\images\MustRead\013.png" style="zoom:100%;" /> |                                                           |


<!-- tab:其它说明 -->

| 说明           | 图示                                                         |
| -------------- | ------------------------------------------------------------ |
| 连线备注或说明 | <img src="\zh-cn\images\MustRead\020.png" alt="image" style="zoom:100%;" /> |

<!-- tabs:end -->



#### 形状示范

##### 功能路径

使用**直角矩形**来表达：

例如：
<!-- tabs:start -->

#### **功能路径流程**

如何进入产品列表如下：

```mermaid
graph LR
   A((系统后台 <div class='in'>开始入口</div>))-->B[产品管理<div class='menu'>菜单位置</div>]-->C[产品列表<div class='menu'>菜单位置</div>]
```

#### **功能路径图示**

<img src="\zh-cn\images\MustRead\list001.png" style="zoom:80%;" />

<!-- tabs:end -->


##### 功能操作

使用**圆角矩形**来表达：

例如：
<!-- tabs:start -->
<!-- tab:功能操作流程 -->

如何添加产品属性：

```mermaid
graph LR
   A((系统后台 <div class='in'>开始入口</div>))-->B[产品管理<div class='menu'>菜单位置</div>]-->C[产品列表<div class='menu'>菜单位置</div>]-->D(添　加 <div class='button'>功能按钮</div>)
```

<!-- tab:功能操作图示 -->
<img src="\zh-cn\images\MustRead\list002.png" style="zoom:80%;" />

<!-- tabs:end -->


#### 功能按钮

使用**体育场形**来表达：

例如：
<!-- tabs:start -->

<!-- tab:功能按钮流程 -->
如何添加产品属性：

```mermaid
graph LR
   A((系统后台 <div class='in'>开始入口</div>))-->B[产品管理<div class='menu'>菜单位置</div>]-->C[产品列表<div class='menu'>菜单位置</div>]-->D(添　加 <div class='button'>功能按钮</div>)-->|完善好表单后|E([保　存 <div class='button'>操作按钮</div>])
```

<!-- tab:功能按钮图示 -->

<img src="\zh-cn\images\MustRead\list003.png" style="zoom:80%;" />

<!-- tabs:end -->



#### 图例串联示范

产品管理的基本功能操作 `之` **管理** 自定义属性

```mermaid
graph TD
0[(OPS系统 <div class='os'>平台入口</div>)]-->A((系统后台 <div class='in'>开始入口</div>)) --> B[产品管理 <div class='menu'>菜单位置</div>]-->C[产品列表 <div class='menu'>菜单位置</div>]---D{产品列表 <div class='list'>数据列表</div>}
D-..-D1>产品1 <div class='one'>单条数据</div>]
D-..-D2>产品2 <div class='one'>单条数据</div>]
D-..-D3>产品...<div class='one'>单条数据</div>]
D2-->|选择所需管理的产品点击|E(操　作<div class='button'>功能按钮</div>)
E---F{菜　单 <div class='list'>数据列表</div>}
F===>|点击| G[[自定义属性 <div class='opt'>可选列表</div>]]
G--->|进入后|H{属性逻辑 <div class='list'>数据列表</div>}
H-..->|1.添加自定义属性|H1(添加属性<div class='button'>功能按钮</div>)
H-..->|2.快捷进入产品属性关联设置|H2(产品属性<div class='button'>功能按钮</div>)
H-..->|3.点击左流程中节点编辑属性|H3(编辑属性<div class='button'>功能按钮</div>)
```


<p align="right">Document creation time:2022-01-26   Update time:{docsify-updated} </p> 
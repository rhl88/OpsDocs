# 企业管理

### 新增企业

### 编辑企业

### 添加管理账户



### 添加下单账户




### 给企业绑定阶梯价格分组
> 系统中每个企业账号都需一个价格分组设置；如果没有设置则使用默认阶梯价格分组。

?> 若企业绑定某个阶梯价格组别后，该企业则以该价格分组中的价格体系进行价格计算。


```mermaid
 graph LR
 0[(OPS系统 <div class='os'>平台入口</div>)]-->1((系统后台<div class='in'>开始入口</div>)) 
  1-.->1-2[企业管理<div class='menu'>菜单位置</div>]
    1-2-->1-2-A[企业列表<div class='menu'>菜单位置</div>]
       1-2-A-.-|选择企业|1-2-A-0-A>企业<div class='one'>单条数据</div>]
       1-2-A-0-A-.->1-2-A-1(操　作<div class='button'>功能按钮</div>)
       1-2-A-1-.->1-2-A-2{菜　单 <div class='list'>数据列表</div>}-.->1-2-B[[修改<div class='opt'>可选列表</div>]]
          1-2-B-.->|选择 阶梯价格分组|1-2-C([保存<div class='button'>操作按钮</div>])
```

### 给企业设置优惠定价分组

> 系统中每个企业账号都需一个优惠定价分组；如果没有设置则使用默认优惠定价分组。

?> 若企业选择了指定的优惠定价分组，该企业结算时将会按分组中关联的产品属性进行折扣计算。
```mermaid
 graph LR
 0[(OPS系统 <div class='os'>平台入口</div>)]-->1((系统后台<div class='in'>开始入口</div>)) 
  1-.->1-2[企业管理<div class='menu'>菜单位置</div>]
    1-2-->1-2-A[企业列表<div class='menu'>菜单位置</div>]
       1-2-A-.-|选择企业|1-2-A-0-A>企业<div class='one'>单条数据</div>]
       1-2-A-0-A-.->1-2-A-1(操　作<div class='button'>功能按钮</div>)
       1-2-A-1-.->1-2-A-2{菜　单 <div class='list'>数据列表</div>}-.->1-2-B[[修改<div class='opt'>可选列表</div>]]
          1-2-B-.->|选择 折扣优惠 关联|1-2-C([保存<div class='button'>操作按钮</div>])
```


### 相互关联功能

- [阶梯价格分组管理](/zh-cn/PricingSystem?id=阶梯价格分组)
- [优惠定价分组管理](/zh-cn/PricingSystem?id=优惠定价分组)

<p align="right">Document creation time:2021-12-17   Update time:{docsify-updated} </p> 
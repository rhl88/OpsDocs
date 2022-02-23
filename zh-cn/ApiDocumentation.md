# 接口使用文档

## Engview

## Product

> 产品

## ReportManager

> 反馈

### 反馈订单制作文件

基本说明



接口信息

| 项目     | 信息                                       | 备注 |
| -------- | ------------------------------------------ | ---- |
| 请求地址 | /api/ReportManager/ReportOrderItemMakeFile |      |
| 请求方式 | POST                                       |      |


请求内容

| Name        | 子项 | 说明 |
| ----------- | ---- | ---- |
| OrderItemNo |      |      |
| FileUrl     |      |      |
| Width       |      |      |
| Height      |      |      |
| NextAction  |      |      |
| FileName    |      |      |
| Num         |      |      |
| SortId      |      |      |

TFLow格式
```json
{
  "OrderItemNo": "{{Item:orderItemNo}}",
  "FileUrl": "UserFiles/WaitFiles/制作后文件/{{Item:MakeFileUrl}}",
  "Width": "{{Item:Width}}",
  "Height":"{{Item:Height}}",
  "NextAction": 2,
  "FileName":"{{$Name}}",
  "Num": "{{Item:num}}",
  "SortId": ""
}
```

### 反馈批次组信息

基本说明



接口信息

| 项目     | 信息                                    | 备注 |
| -------- | --------------------------------------- | ---- |
| 请求地址 | /api/ReportManager/ReportBatchGroupInfo |      |
| 请求方式 | POST                                    |      |


请求内容

| Name           | 子项            | 说明 |
| -------------- | --------------- | ---- |
| BatchName      |                 |      |
| GroupFileInfos |                 |      |
|                | GroupId         |      |
|                | PaperName       |      |
|                | BarCodeList     |      |
|                | BarCodeInfos    |      |
|                | FileName        |      |
|                | FileSize        |      |
|                | FileUrl         |      |
|                | PreviewFileUrl  |      |
|                | Printer         |      |
|                | Sides           |      |
|                | Size            |      |
|                | PrintColor      |      |
|                | RunLength       |      |
|                | CoordinateInfos |      |
|                | Remark          |      |

TFLow格式
```json
{
  "BatchName": "{{Instance:batchName}}",
  "GroupFileInfos": [
    {
      "GroupId": "{{Item:GroupID}}",
      "PaperName": "{{Instance:material}}",
      "BarCodeList": [
        {{Instance:barcodeList}}      ],
      "BarCodeInfos": {{Instance:barcodeInfos}},
      "FileName": "{{$ClearName}}",
      "FileSize": 0,
      "FileUrl": "/ImposeResult{{Item:imposeUrl}}",
      "PreviewFileUrl": "string",
      "Printer":"{{Instance:printer}}",
      "Sides":"{{Instance:duplex}}",
      "Size": "{{Item:Size}}",
      "PrintColor": "{{Instance:color}}",
      "RunLength":'{{Item:finalNum}}',
      "CoordinateInfos": [
      ],
      "Remark":"{{Item:remark}}"
    }
  ]
}
```


### 报错反馈

基本说明




接口信息

| 项目     | 信息                                         | 备注 |
| -------- | -------------------------------------------- | ---- |
| 请求地址 | /api/ReportManager/ReportBatchGroupErrorInfo |      |
| 请求方式 | POST                                         |      |

请求内容

| Name         | 子项 | 说明       |
| ------------ | ---- | ---------- |
| BatchName    |      | 销售订单号 |
| ErrorMessage |      | 错误信息   |

TFLow格式
```json
{
  "BatchName": "{{Instance:saleOrderNo}}",
  "ErrorMessage": "{{Instance:errNote}}"
}
```

## SaleOrder

> 订单

### 开单请求

基本说明



接口信息

| 项目     | 信息                           | 备注 |
| -------- | ------------------------------ | ---- |
| 请求地址 | /api/SaleOrder/CreateSaleOrder |      |
| 请求方式 | POST                           |      |

请求内容

| Name                 | 子项     | 说明 |
| -------------------- | -------- | ---- |
| Title                |          |      |
| MemberId             |          |      |
| ProductItemNo        |          |      |
| OrderItemNum         |          |      |
| SaleOrderNo          |          |      |
| AddressBookId        |          |      |
| AddressBookInfo      |          |      |
|                      | LinkMan  |      |
|                      | Province |      |
|                      | City     |      |
|                      | County   |      |
|                      | Address  |      |
|                      | Postcode |      |
|                      | Mobile   |      |
|                      | Tel      |      |
| ProductPropertyCodes |          |      |
| OrderItemInfos       |          |      |
| paper                |          |      |
| PropertyNodeEncrypt  |          |      |

TFLow格式
```json
{
  "Title": "{{Instance:orgName}}",
  "MemberId": "{{Xml:/JDF/memberId}}",
  "ProductItemNo": "{{Xml:/JDF/production/prodCode}}",
  "OrderItemNum": "",
  "SaleOrderNo":"{{Xml:/JDF/saleOrderNo}}",
  "AddressBookId":"",
  "AddressBookInfo": {
    "LinkMan": "{{Xml:/JDF/receiverName}}",
    "Province": "{{Xml:/JDF/province}}",
    "City": "{{Xml:/JDF/city}}",
    "County": "{{Xml:/JDF/county}}",
    "Address": "{{Xml:/JDF/address}}",
    "Postcode":"510000",
    "Mobile": "{{Xml:/JDF/receiverMobile}}",
    "Tel": ""
    },
  "ProductPropertyCodes":"",
  "OrderItemInfos":[{{Instance:jsonInstance}}],
  "paper":"{{Instance:paper}}",
  "PropertyNodeEncrypt":"{{Xml:/JDF/PropertyInfoEncrypt}}"
}
```

### 反馈订单项目组

基本说明



接口信息

| 项目     | 信息                                | 备注 |
| -------- | ----------------------------------- | ---- |
| 请求地址 | /api/SaleOrder/ReportOrderItemGroup |      |
| 请求方式 | POST                                |      |

请求内容

| Name          | 子项 | 说明 |
| ------------- | ---- | ---- |
| PrinterName   |      |      |
| SupplierCode  |      |      |
| GroupPdfName  |      |      |
| GroupId       |      |      |
| GroupPdfUrl   |      |      |
| Type          |      |      |
| Area          |      |      |
| PaperName     |      |      |
| BarCodeList   |      |      |
| CatalogName   |      |      |
| PdfPreviewUrl |      |      |
| BatchName     |      |      |
| RunLength     |      |      |
| Remark        |      |      |
| PageNum       |      |      |
| Size          |      |      |
| Sides         |      |      |
| Color         |      |      |
| Status        |      |      |

TFLow格式
```json
{
  "PrinterName": "{{Instance:printer}}",
  "SupplierCode": "{{Instance:supplierCode}}",
  "GroupPdfName": "{{$ClearName}}",
  "GroupId": "{{Item:GroupID}}",
  "GroupPdfUrl": "/ImposeResult{{Item:imposeUrl}}",
  "Type": "普通",
  "Area": "杭州",
  "PaperName": "{{Instance:material}}",
  "BarCodeList": [
    {{Instance:barcodeList}}
  ],
  "CatalogName": "普通",
  "PdfPreviewUrl": "/ImposeResult/{{Date:yyyyMMdd}}/{{$Name}}",
  "BatchName": "{{Instance:batchName}}",
  "RunLength": "{{Item:finalNum}}",
  "Remark": "{{Item:remark}}",
  "PageNum": "{{Item:pgCount}}",
  "Size": "{{Item:Size}}",
  "Sides": "{{Instance:duplex}}",
  "Color": "{{Instance:color}}",
  "Status":0
}

```

### 反馈订单组状态

基本说明



接口信息

| 项目     | 信息                             | 备注 |
| -------- | -------------------------------- | ---- |
| 请求地址 | /api/SaleOrder/ReportGroupStatus |      |
| 请求方式 | POST                             |      |

请求内容

| Name         | 子项       | 说明                       |
| ------------ | ---------- | -------------------------- |
| SupplierCode |            |                            |
|              | IY8MXDELA4 | 发送打印反馈               |
| GroupId      |            |                            |
| Status       |            |                            |
|              | 1          |                            |
|              | 2          |                            |
|              | 3          |                            |
|              | 4          | 待操作打印(待打印)         |
|              | 5          | 文件发送打印机中（移动中） |
|              | 6          | 已发送打印机（已打印）     |
|              | 10         | 已上机印刷（已上机）       |
|              | 11         | 已撤销                     |

TFLow格式
```json
{
  "SupplierCode": "IY8MXDELA4",
  "GroupId": "{{Instance:groupId}}",
  "Status": 6
}
```

## Stat

## System

> 系统

## Express

## Swagger



<p align="right">Document creation time:2021-12-29   Update time:{docsify-updated} </p> 
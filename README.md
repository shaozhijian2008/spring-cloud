 ##  项目报备提交      
* 请求路径 : /oss/project/api/add
* 接口所在类 : ProjectFilingController

> 请求参数说明

| 字段名称 | 字段中文名称 | 是否必须 | 说明 |
| ---- | ---- | ---- | ---- |
| weixinName | 微信昵称 | Y | 微信昵称 |
| reporterId | 分销系统内的用户id | Y | 分销系统内的用户id |
| reporter | 姓名 | Y | 提交人姓名 |
| phone | 手机号 | Y | 手机号 |
| industryType | 项目行业类型 | Y | 项目行业类型 |
| industry | 项目行业 | Y | 项目行业 |
| refCorporation | 公司名称 | Y | 公司名称 |
| state | 项目说明 | N | 项目说明 |
| fileName | 附件名称 | Y | 附件名称 |
| filePath | 附件url | Y | 附件url  |
| fileBase64 | 附件base64 | N | 附件base64编码数据 |
	

> 返回内容说明

| 字段名称 | 字段中文名称 | 是否必须 | 说明 |


> 返回内容范例

```
{
    "message":"新增成功!",
    "code":"200"
}
```

 ## 我的报备总数      
* 请求路径 : /oss/project/api/count
* 接口所在类 : ProjectFilingController

> 请求参数说明

| 字段名称 | 字段中文名称 | 是否必须 | 说明 |
| ---- | ---- | ---- | ---- |
| reporterId | 分销系统内的用户id | Y | 分销系统内的用户id |
	

> 返回内容说明

| 字段名称 | 字段中文名称 | 是否必须 | 说明 |


> 返回内容范例

```
{
    "message":"查询成功!",
    "result":5,
    "code":"200"
}
```

 ## 我的报备列表      
* 请求路径 : /oss/project/api/list
* 接口所在类 : ProjectFilingController

> 请求参数说明

| 字段名称 | 字段中文名称 | 是否必须 | 说明 |
| ---- | ---- | ---- | ---- |
| reporterId | 分销系统内的用户id | Y | 分销系统内的用户id |
| pageIndex | 查询页数 | Y | 查询页数 |
| pageSize | 分页显示条数 | Y | 分页显示条数 |
	

> 返回内容说明

| 字段名称 | 字段中文名称 | 是否必须 | 说明 |
| ---- | ---- | ---- | ---- |
| reportDate | 报备日期 | Y | 报备日期 |
| status | 状态 | Y | 0:未跟进 1:已跟进 2:已作废 |
| reporter | 姓名 | Y | 提交人姓名 |
| phone | 手机号 | Y | 手机号 |
| industryType | 项目行业类型 | Y | 项目行业类型 |
| industry | 项目行业 | Y | 项目行业 |
| refCorporation | 公司名称 | Y | 公司名称 |
| state | 项目说明 | N | 项目说明 |
| fileName | 附件名称 | Y | 附件名称 |



> 返回内容范例

```
{
    "message":"查询成功!",
    "result":[{"status":0,"industryType":"整车销售","industry":"汽车贸易","reportDate":"2017/10/18 10:28","reporter":"张三","phone":"12345678910","refCorporation":"杭州屹车有限公司","state":"项目说明","fileName":"XXXXX.png"}],
    "code":"200"
}
```

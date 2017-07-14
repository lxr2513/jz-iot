# 获取上行数据

```js
GET /v1/application/data?appeui=1234561231312312&token=cf2e793103a448c2b46dc1c18c3d1995&order=desc
```

## 

## 请求参数

| **参数名称** | **参数描述** | **数据类型** | **是否必填** |
| :---: | :---: | :---: | :---: |
| qppeui | 应用EUI | string | N/Y |
| deveui | 设备EUI | string | N/Y |
| token | 密钥 | string | Y |
| start | 查询数据的开始时间\(自1970零时刻以来毫秒数\) | number | N |
| end | 查询数据的结束时间\(自1970零时刻以来毫秒数\) | number | N |
| limit | 最大查询数量（默认1000） | number | N |
| offset | 查询数据偏移量 | number | N |
| order | 返回数据按时间的排序\[asc,desc\]，默认desc | string | N |



## 响应参数

| **参数名称** | **参数描述** | **数据类型** | **是否必填** |
| :---: | :---: | :---: | :---: |
| createDate | 数据接收时间 | Date | Y |
| appEUI | 应用EUI | string | Y |
| bandwidth | 带宽 | number | Y |
| datarate | 数据速率 | number | Y |
| channel | 频道 | string | Y |
| codr | ECC码率 | number | Y |
| crcstatus | CRC状态 | number | Y |
| data | 数据 | string | Y |
| devEUI | 设备EUI | string | Y |
| moteId | 设备Id | number | Y |
| dataType | 数据类型（0下行，1上行） | string | Y |
| fcnt | 包计数器 | number | Y |
| fctrl | 帧数速率控制 | number | Y |
| fopts | 传输MAC命令 | number | Y |
| port | 数据接收端口 | number | Y |
| freq | 无线频率 | number | Y |
| gwEUI | 网关EUI | string | Y |
| lsnr | 信噪比 | string | Y |
| modulation | 调制方式 | string | Y |
| mtype | MAc命令类型 | number | Y |
| org |  | string | Y |
| rfchain |  | string | Y |
| rssi | 信号强度 | number | Y |
| size | 长度 | number | Y |
| SF | 扩频因子 | number | Y |



## JSON对象实例

\[{

	"createDate": "2017-06-13T05:34:20.000Z",

	"appEUI": "0e01010101010101",

	"bandwidth": 125,

	"datarate": 0,

	"channel": null,

	"codr": "4/5",

	"crcstatus": 0,

	"data": "41 1",

	"devEUI": "be7a0000000005ea",

	"moteId": 20,

	"dataType": 0,

	"fcnt": 0,

	"fctrl": "0",

	"fopts": "",

	"port": 99,

	"freq": 476,

	"gwEUI": null,

	"lsnr": null,

	"modulation": "LORA",

	"mtype": "",

	"org": 0,

	"rfchain": 1,

	"rssi": null,

	"size": 0,

	"SF": 12

}\]




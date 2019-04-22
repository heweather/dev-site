---
book: API
service: api
data: alarm
version: 6.1
title: 天气灾害预警
toc: true
description: 本接口可获取全国全国3240个市县区所有天气灾害预警信息。

---

## 数据介绍

- 获取当前时间点全国3240个市县区所有灾害预警信息。
- 预警种类：台风、暴雨、暴雪、寒潮、大风、沙尘暴、高温、干旱、雷电、冰雹、霜冻、大雾、霾、道路结冰、寒冷、灰霾、雷雨大风、森林火险、降温、道路冰雪、干热风、低温、冰冻、空气重污染、海上大雾、雷暴大风、持续低温、浓浮尘、龙卷风、低温冻害、海上大风、低温雨雪冰冻、强对流、臭氧、大雪、强降雨、强降温、雪灾、森林（草原）火险、雷暴、严寒、沙尘、海上雷雨大风、海上雷电、海上台风。
- 预警级别：白色（仅限广东省内）、蓝色、黄色、橙色、红色
- 更新时间：每15分钟更新一次。

> - 当使用此接口时，会按照返回的预警数量扣除相应的访问量

## 请求URL

**商业版(指定地区）：**
```
https://api.heweather.net/s6/alarm?{parameters}
```
**商业版(全部地区）：**
```
https://api.heweather.net/s6/alarm/all?{parameters}
```

- `{parameters}`代表请求参数，包括必选和可选参数。所有请求参数均使用 `&`进行分隔，参数值存在中文或特殊字符的情况，需要对参数进行 **url encode**。

> 请注意，在替换`{parameters}`对应值的时候，URL中不要包含大括号`{}`

### 请求URL示例
```
# 获取北京的灾害预警信息
https://api.heweather.net/s6/alarm/location=beijing&key=xxx
```

## 请求参数

| 参数 | 描述                                                         | 选择 | 示例值             |
| ---- | ------------------------------------------------------------ | ---- | ------------------ |
| lang | 多语言，可以不使用该参数，默认为简体中文<br>详见[多语言参数](/docs/refer/i18n) | 可选 | lang=en            |
| unit | 单位选择，公制（m）或英制（i），默认为公制单位<br>详见[度量衡单位参数](/docs/refer/unit) | 可选 | unit=i             |
| key  | 用户数据key，请参考[如何获取你的KEY](https://www.heweather.com/support/setup-app-key)<br>支持[数字签名](/docs/sercet-authorization)方式进行认证，推荐使用 | 必选 | key=xxxxxxxxxxxxxx |

## 数据返回字段和数值说明

### `update` 接口更新时间

| 参数 | 描述                                     | 示例值           |
| ---- | ---------------------------------------- | ---------------- |
| loc  | 当地时间，24小时制，格式yyyy-MM-dd HH:mm | 2017-10-25 12:34 |
| utc  | UTC时间，24小时制，格式yyyy-MM-dd HH:mm  | 2017-10-25 04:34 |

### `status` 接口状态

| 参数   | 描述                                                         | 示例 |
| ------ | ------------------------------------------------------------ | ---- |
| status | 接口状态，具体含义请参考[接口状态码及错误码](/docs/refer/status-code) | ok   |

### `alarm_list` 灾害预警

| 参数  | 描述         | 示例                                                         |
| ----- | ------------ | ------------------------------------------------------------ |
| cid   | 地区／城市ID | CN101280601                                                  |
| title | 预警信息标题 | 广东省深圳市气象台发布雷电黄色预警                           |
| stat  | 预警状态     | 预警中                                                       |
| level | 预警等级     | 黄色                                                         |
| type  | 预警类型     | 雷电                                                         |
| txt   | 预警详细信息 | 深圳市气象局于10月04日12时59分发布雷电黄色预警信号，请注意防御。 |

## 数据返回示例

```json
{
    "HeWeather6": {
        "alarm_list": [
            {
                "cid": "CN101050110",
                "level": "蓝色",
                "stat": "预警中",
                "title": "黑龙江省哈尔滨市延寿县气象台发布大风蓝色预警",
                "txt": "预计未来24小时内延寿地区将受大风影响,平均风力可达6级以上，或者阵风7级以上。请有关单位和个人注意做好预防工作。\n",
                "type": "大风"
            },
            {
                "cid": "CN101050110",
                "level": "蓝色",
                "stat": "预警中",
                "title": "黑龙江省哈尔滨市气象台发布大风蓝色预警",
                "txt": "哈尔滨市气象台2018年4月16日15:20发布大风蓝色预警信号：预计16日下午至17日白天哈尔滨主城区及各区、县（市）将受大风影响，平均风力4-6级，阵风7-8级，火险等级高，请注意防范。",
                "type": "大风"
            },
            {
                "cid": "CN101050111",
                "level": "蓝色",
                "stat": "预警中",
                "title": "黑龙江省哈尔滨市尚志市气象台发布大风蓝色预警",
                "txt": "尚志市气象局2018年4月16日16时20分发布大风蓝色预警：预计未来24小时尚志地区将受大风影响,平均风力4-5级，阵风可达6-7级。请有关单位和个人注意做好预防工作。",
                "type": "大风"
            },
            {
                "cid": "CN101050111",
                "level": "蓝色",
                "stat": "预警中",
                "title": "黑龙江省哈尔滨市气象台发布大风蓝色预警",
                "txt": "哈尔滨市气象台2018年4月16日15:20发布大风蓝色预警信号：预计16日下午至17日白天哈尔滨主城区及各区、县（市）将受大风影响，平均风力4-6级，阵风7-8级，火险等级高，请注意防范。",
                "type": "大风"
            },
            {
                "cid": "CN101050112",
                "level": "蓝色",
                "stat": "预警中",
                "title": "黑龙江省哈尔滨市五常市气象台发布大风蓝色预警",
                "txt": "五常市气象台4月16日18时40分发布大风蓝色预警信号：预计未来24小时五常地区将受大风影响，平均风力4-6级，阵风7-8级，火险等级高，请注意防范。",
                "type": "大风"
            },
            {
                "cid": "CN101050112",
                "level": "蓝色",
                "stat": "预警中",
                "title": "黑龙江省哈尔滨市气象台发布大风蓝色预警",
                "txt": "哈尔滨市气象台2018年4月16日15:20发布大风蓝色预警信号：预计16日下午至17日白天哈尔滨主城区及各区、县（市）将受大风影响，平均风力4-6级，阵风7-8级，火险等级高，请注意防范。",
                "type": "大风"
            },
            {
                "cid": "CN101050113",
                "level": "蓝色",
                "stat": "预警中",
                "title": "黑龙江省哈尔滨市木兰县气象台发布大风蓝色预警",
                "txt": "木兰县气象台2018年4月16日16时00分发布大风蓝色预警信号：预计16日下午至17日白天我县将受大风影响，平均风力4-6级，阵风7-8级，火险等级高，请注意防范。",
                "type": "大风"
            },
            {
                "cid": "CN101050113",
                "level": "蓝色",
                "stat": "预警中",
                "title": "黑龙江省哈尔滨市气象台发布大风蓝色预警",
                "txt": "哈尔滨市气象台2018年4月16日15:20发布大风蓝色预警信号：预计16日下午至17日白天哈尔滨主城区及各区、县（市）将受大风影响，平均风力4-6级，阵风7-8级，火险等级高，请注意防范。",
                "type": "大风"
            },
            {
                "cid": "CN101050201",
                "level": "蓝色",
                "stat": "预警中",
                "title": "黑龙江省气象台发布大风蓝色预警",
                "txt": " 黑龙江省气象台4月16日15时40分发布大风蓝色预警信号：预计未来24小时齐齐哈尔南部、大庆、绥化、哈尔滨、伊春南部、佳木斯、双鸭山、七台河、鸡西、牡丹江将自西向东逐渐受大风影响,平均风力5级，阵风7级左右,其它地区平均风力3-4级。请有关单位和个人注意做好预防工作。",
                "type": "大风"
            },
            {
                "cid": "CN101050101",
                "level": "蓝色",
                "stat": "预警中",
                "title": "黑龙江省气象台发布大风蓝色预警",
                "txt": " 黑龙江省气象台4月16日15时40分发布大风蓝色预警信号：预计未来24小时齐齐哈尔南部、大庆、绥化、哈尔滨、伊春南部、佳木斯、双鸭山、七台河、鸡西、牡丹江将自西向东逐渐受大风影响,平均风力5级，阵风7级左右,其它地区平均风力3-4级。请有关单位和个人注意做好预防工作。",
                "type": "大风"
            },
            {
                "cid": "CN101290905",
                "level": "黄色",
                "stat": "预警中",
                "title": "云南省普洱市思茅区气象台发布雷电黄色预警",
                "txt": "思茅区气象台2018年4月16日16时25分发布雷电黄色预警信号：预计未来6小时内思茅区将出现雷电活动，局部伴有冰雹、大风等强对流天气，请注意防范。",
                "type": "雷电"
            }
        ],
        "status": "ok",
        "update": {
            "loc": "2018-04-17 10:36",
            "utc": "2018-04-17 02:36"
        }
    }
}
```
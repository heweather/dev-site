---
title: 逐小时预报（未来24小时）
---
{:.pre-scrollable}
```
// 北京未来24小时逐小时天气 
// 商业版 https://api.qweather.com/v7/weather/24d?location=101010100&key=xxx
// 开发版 https://devapi.qweather.com/v7/weather/24d?location=101010100&key=xxx
// 请将示例请求URL中的KEY更换成你自己的KEY

{
  "code": "200",
  "updateTime": "2020-06-14T17:09+08:00",
  "fxLink": "https://www.qweather.com/weather/beijing-101010100.html",
  "hourly": [
    {
      "fxDate": "2020-06-14T18:00+08:00",
      "temp": "34",
      "icon": "150",
      "text": "晴",
      "wind360": "101",
      "windDir": "东南风",
      "windScale": "3-4",
      "windSpeed": "14",
      "humidity": "19",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1001",
      "cloud": "6",
      "dew": "3",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-14T19:00+08:00",
      "temp": "33",
      "icon": "150",
      "text": "晴",
      "wind360": "153",
      "windDir": "东南风",
      "windScale": "1-2",
      "windSpeed": "1",
      "humidity": "22",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1001",
      "cloud": "3",
      "dew": "4",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-14T20:00+08:00",
      "temp": "30",
      "icon": "150",
      "text": "晴",
      "wind360": "355",
      "windDir": "北风",
      "windScale": "1-2",
      "windSpeed": "6",
      "humidity": "24",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1001",
      "cloud": "0",
      "dew": "5",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-14T21:00+08:00",
      "temp": "29",
      "icon": "150",
      "text": "晴",
      "wind360": "173",
      "windDir": "南风",
      "windScale": "3-4",
      "windSpeed": "21",
      "humidity": "28",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1002",
      "cloud": "0",
      "dew": "5",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-14T22:00+08:00",
      "temp": "27",
      "icon": "150",
      "text": "晴",
      "wind360": "214",
      "windDir": "西南风",
      "windScale": "1-2",
      "windSpeed": "10",
      "humidity": "32",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1002",
      "cloud": "0",
      "dew": "5",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-14T23:00+08:00",
      "temp": "26",
      "icon": "150",
      "text": "晴",
      "wind360": "245",
      "windDir": "西南风",
      "windScale": "1-2",
      "windSpeed": "9",
      "humidity": "37",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1002",
      "cloud": "0",
      "dew": "4",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T00:00+08:00",
      "temp": "25",
      "icon": "150",
      "text": "晴",
      "wind360": "274",
      "windDir": "西风",
      "windScale": "1-2",
      "windSpeed": "1",
      "humidity": "37",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1002",
      "cloud": "5",
      "dew": "5",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T01:00+08:00",
      "temp": "24",
      "icon": "150",
      "text": "晴",
      "wind360": "279",
      "windDir": "西风",
      "windScale": "1-2",
      "windSpeed": "3",
      "humidity": "38",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1002",
      "cloud": "9",
      "dew": "5",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T02:00+08:00",
      "temp": "23",
      "icon": "150",
      "text": "晴",
      "wind360": "242",
      "windDir": "西南风",
      "windScale": "1-2",
      "windSpeed": "9",
      "humidity": "39",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1002",
      "cloud": "14",
      "dew": "5",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T03:00+08:00",
      "temp": "22",
      "icon": "150",
      "text": "晴",
      "wind360": "266",
      "windDir": "西风",
      "windScale": "1-2",
      "windSpeed": "10",
      "humidity": "41",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1001",
      "cloud": "9",
      "dew": "6",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T04:00+08:00",
      "temp": "22",
      "icon": "150",
      "text": "晴",
      "wind360": "276",
      "windDir": "西风",
      "windScale": "1-2",
      "windSpeed": "9",
      "humidity": "43",
      "pop": "0",
      "precip": "0.0",
      "pressure": "1000",
      "cloud": "5",
      "dew": "6",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T05:00+08:00",
      "temp": "22",
      "icon": "150",
      "text": "晴",
      "wind360": "207",
      "windDir": "西南风",
      "windScale": "1-2",
      "windSpeed": "6",
      "humidity": "46",
      "pop": "0",
      "precip": "0.0",
      "pressure": "999",
      "cloud": "0",
      "dew": "5",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T06:00+08:00",
      "temp": "25",
      "icon": "150",
      "text": "晴",
      "wind360": "266",
      "windDir": "西风",
      "windScale": "1-2",
      "windSpeed": "3",
      "humidity": "42",
      "pop": "0",
      "precip": "0.0",
      "pressure": "998",
      "cloud": "13",
      "dew": "7",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T07:00+08:00",
      "temp": "26",
      "icon": "150",
      "text": "晴",
      "wind360": "154",
      "windDir": "东南风",
      "windScale": "1-2",
      "windSpeed": "6",
      "humidity": "38",
      "pop": "0",
      "precip": "0.0",
      "pressure": "998",
      "cloud": "25",
      "dew": "7",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T08:00+08:00",
      "temp": "27",
      "icon": "150",
      "text": "晴",
      "wind360": "238",
      "windDir": "西南风",
      "windScale": "1-2",
      "windSpeed": "1",
      "humidity": "34",
      "pop": "0",
      "precip": "0.0",
      "pressure": "997",
      "cloud": "38",
      "dew": "6",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T09:00+08:00",
      "temp": "29",
      "icon": "150",
      "text": "晴",
      "wind360": "136",
      "windDir": "东南风",
      "windScale": "1-2",
      "windSpeed": "8",
      "humidity": "31",
      "pop": "0",
      "precip": "0.0",
      "pressure": "997",
      "cloud": "55",
      "dew": "5",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T10:00+08:00",
      "temp": "31",
      "icon": "150",
      "text": "晴",
      "wind360": "118",
      "windDir": "东南风",
      "windScale": "1-2",
      "windSpeed": "5",
      "humidity": "29",
      "pop": "0",
      "precip": "0.0",
      "pressure": "997",
      "cloud": "72",
      "dew": "3",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T11:00+08:00",
      "temp": "33",
      "icon": "150",
      "text": "晴",
      "wind360": "7",
      "windDir": "北风",
      "windScale": "1-2",
      "windSpeed": "10",
      "humidity": "26",
      "pop": "0",
      "precip": "0.0",
      "pressure": "997",
      "cloud": "90",
      "dew": "2",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T12:00+08:00",
      "temp": "34",
      "icon": "150",
      "text": "晴",
      "wind360": "279",
      "windDir": "西风",
      "windScale": "1-2",
      "windSpeed": "1",
      "humidity": "24",
      "pop": "0",
      "precip": "0.0",
      "pressure": "997",
      "cloud": "91",
      "dew": "0",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T13:00+08:00",
      "temp": "35",
      "icon": "150",
      "text": "晴",
      "wind360": "249",
      "windDir": "西南风",
      "windScale": "1-2",
      "windSpeed": "5",
      "humidity": "23",
      "pop": "0",
      "precip": "0.0",
      "pressure": "998",
      "cloud": "93",
      "dew": "0",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T14:00+08:00",
      "temp": "35",
      "icon": "150",
      "text": "晴",
      "wind360": "0",
      "windDir": "北风",
      "windScale": "1-2",
      "windSpeed": "1",
      "humidity": "21",
      "pop": "0",
      "precip": "0.0",
      "pressure": "998",
      "cloud": "95",
      "dew": "0",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T15:00+08:00",
      "temp": "35",
      "icon": "150",
      "text": "晴",
      "wind360": "128",
      "windDir": "东南风",
      "windScale": "1-2",
      "windSpeed": "7",
      "humidity": "20",
      "pop": "0",
      "precip": "0.0",
      "pressure": "998",
      "cloud": "93",
      "dew": "0",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T16:00+08:00",
      "temp": "35",
      "icon": "150",
      "text": "晴",
      "wind360": "165",
      "windDir": "东南风",
      "windScale": "1-2",
      "windSpeed": "11",
      "humidity": "20",
      "pop": "0",
      "precip": "0.0",
      "pressure": "999",
      "cloud": "91",
      "dew": "0",
      "snow": "0.0",
      "ice": "0.0"
    },
    {
      "fxDate": "2020-06-15T17:00+08:00",
      "temp": "36",
      "icon": "150",
      "text": "晴",
      "wind360": "8",
      "windDir": "北风",
      "windScale": "1-2",
      "windSpeed": "6",
      "humidity": "20",
      "pop": "0",
      "precip": "0.0",
      "pressure": "999",
      "cloud": "89",
      "dew": "0",
      "snow": "0.0",
      "ice": "0.0"
    }
  ],
  "refer": {
    "sources": [
      "Weather China"
    ],
    "license": [
      "commercial license"
    ]
  }
}
```
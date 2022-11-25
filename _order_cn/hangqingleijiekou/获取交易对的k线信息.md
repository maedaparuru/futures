---
title: 获取交易对的k线信息
position_number: 8
type: get
split: '-------------------------------------'
description: |
    接口地址:/v1/public/q/kline<br>
    请求方式:GET<br>
    请求数据类型:application/x-www-form-urlencoded<br>
    响应数据类型:*/*
parameters:
    -
        name:
        type:
        mandatory: false
        default:
        description:
        ranges:
content_markdown: |-
    **请求参数**\:

    | 参数名称 | 参数说明 | 请求类型 | 是否必须 | 数据类型 | schema |
    | --- | --- | --- | --- | --- | --- |
    | interval | 时间间隔 | query | true | string | &nbsp; |
    | symbol | 交易对 | query | true | string | &nbsp; |
    | endTime | 结束时间 | query | false | integer(int64) | &nbsp; |
    | limit | 限制条数 | query | false | integer(int32) | &nbsp; |
    | startTime | 起始时间 | query | false | integer(int64) | &nbsp; |

    **响应状态**\:

    | 状态码 | 说明 | schema |
    | --- | --- | --- |
    | 200 | OK | CommonResponse&laquo;List&laquo;KlineVO&raquo;&raquo; |
    | 401 | Unauthorized | &nbsp; |
    | 403 | Forbidden | &nbsp; |
    | 404 | Not Found | &nbsp; |

    **响应参数**\:

    | 参数名称 | 参数说明 | 类型 | schema |
    | --- | --- | --- | --- |
    | error | &nbsp; | ErrorMessage | ErrorMessage |
    | code | &nbsp; | string | &nbsp; |
    | msg | &nbsp; | string | &nbsp; |
    | msgInfo | &nbsp; | string | &nbsp; |
    | result | &nbsp; | array | KlineVO |
    | a | 成交量 | number(bigdecimal) | &nbsp; |
    | c | 结束价 | number(bigdecimal) | &nbsp; |
    | h | 最高价 | number(bigdecimal) | &nbsp; |
    | l | 最低价 | number(bigdecimal) | &nbsp; |
    | o | 开始价 | number(bigdecimal) | &nbsp; |
    | s | 交易对 | string | &nbsp; |
    | t | 时间 | integer(int64) | &nbsp; |
    | v | 成交额 | number(bigdecimal) | &nbsp; |
    | returnCode | &nbsp; | integer(int32) | integer(int32) |

    &nbsp;

    &nbsp;
left_code_blocks:
    -
        code_block:
        title:
        language:
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": [\n\t\t{\n\t\t\t\"a\": 0,\n\t\t\t\"c\": 0,\n\t\t\t\"h\": 0,\n\t\t\t\"l\": 0,\n\t\t\t\"o\": 0,\n\t\t\t\"s\": \"\",\n\t\t\t\"t\": 0,\n\t\t\t\"v\": 0\n\t\t}\n\t],\n\t\"returnCode\": 0\n}"
        title: Response
        language: javascript
---

---
title: 响应代码
position_number: 9
parameters:
    -
        name:
content:
content_markdown: |-
    | httpStatus | 描述 |
    | --- | --- |
    | 200 | 请求成功，请进一步查看rc、mc部分 |
    | 404 | 接口不存在 |
    | 429 | 请求过于频繁，请按照限速要求，控制请求速率 |
    | 500 | 服务异常 |
    | 502 | 网关异常 |
    | 503 | 服务不可用，请稍后重试 |

    | rc | return Code |
    | --- | --- |
    | 0 | 业务成功 |
    | 1 | 业务失败 |

    | mc | message code |
    | --- | --- |
    | SUCCESS | 成功 |
    | FAILURE | 失败 |
    | AUTH\_001 | 缺少请求头 x-validate-appkey |
    | AUTH\_002 | 缺少请求头 x-validate-timestamp |
    | AUTH\_003 | 缺少请求头 x-validate-recvwindow |
    | AUTH\_004 | 错误的请求头 x-validate-recvwindow |
    | AUTH\_005 | 缺少请求头 x-validate-algorithms |
    | AUTH\_006 | 错误的请求头 x-validate-algorithms |
    | AUTH\_007 | 缺少请求头 x-validate-signature |
    | AUTH\_101 | ApiKey不存在 |
    | AUTH\_102 | ApiKey未激活 |
    | AUTH\_103 | 签名错误 |
    | AUTH\_104 | 非绑定IP请求 |
    | AUTH\_105 | 报文过时 |
    | AUTH\_106 | 超出apikey权限 |
    | SYMBOL\_001 | 交易对不存在 |
    | SYMBOL\_002 | 交易对未开盘 |
    | SYMBOL\_003 | 交易对暂停交易 |
    | SYMBOL\_004 | 此交易对不支持您所在的国家 |
    | ORDER\_001 | 平台拒单 |
    | ORDER\_002 | 资金不足 |
    | ORDER\_003 | 交易对暂停交易 |
    | ORDER\_004 | 禁止交易 |
    | ORDER\_005 | 订单不存在 |
    | ORDER\_006 | 过多的未完成订单 |
    | ORDER\_F0101 | 触发价格过滤器-最小值 |
    | ORDER\_F0102 | 触发价格过滤器-最大值 |
    | ORDER\_F0103 | 触发价格过滤器-步进值 |
    | ORDER\_F0201 | 触发数量过滤器-最小值 |
    | ORDER\_F0202 | 触发数量过滤器-最大值 |
    | ORDER\_F0203 | 触发数量过滤器-步进值 |
    | ORDER\_F0301 | 触发金额过滤器-最小值 |
    | ORDER\_F0401 | 触发开盘保护滤器 |
    | ORDER\_F0501 | 触发限价保护滤器 |
    | ORDER\_F0601 | 触发市价保护滤器 |
left_code_blocks:
    -
        code_block:
        title:
        language:
        right_code_blocks:
    -
        code_block:
        title:
        language:
---

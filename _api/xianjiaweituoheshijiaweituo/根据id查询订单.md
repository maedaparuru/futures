---
title: 根据id查询订单
position_number: 7
type: get
split: '-------------------------------------'
description: |+
    接口地址:/v1/order/detail<br>
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
content_markdown: >-
    **请求参数**\:


    | 参数名称 | 参数说明 | 请求类型 | 是否必须 | 数据类型 | schema |

    | --- | --- | --- | --- | --- | --- |

    | orderId | orderId | query | true | integer(int64) | &nbsp; |


    **响应状态**\:


    | 状态码 | 说明 | schema |

    | --- | --- | --- |

    | 200 | OK | CommonResponse&laquo;OrderVO&raquo; |

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

    | result | &nbsp; | OrderVO | OrderVO |

    | avgPrice | 成交均价 | number(bigdecimal) | &nbsp; |

    | clientOrderId | 自定义订单id | string | &nbsp; |

    | closePosition | 是否条件全平仓 | boolean | &nbsp; |

    | closeProfit | 平仓盈亏 | number(bigdecimal) | &nbsp; |

    | createdTime | 创建时间 | integer(int64) | &nbsp; |

    | executedQty | 已成交数量（张） | number(bigdecimal) | &nbsp; |

    | forceClose | 是否是全平订单 | boolean | &nbsp; |

    | marginFrozen | 占用保证金 | number(bigdecimal) | &nbsp; |

    | orderId | 订单id | integer(int64) | &nbsp; |

    | orderSide | 买卖方向 | string | &nbsp; |

    | orderType | 订单类型 | string | &nbsp; |

    | origQty | 数量（张） | number(bigdecimal) | &nbsp; |

    | positionSide | 持仓方向 | string | &nbsp; |

    | price | 委托价格 | number(bigdecimal) | &nbsp; |

    | sourceId | 条件触发id | integer(int64) | &nbsp; |

    | state | 订单状态
    NEW：新建订单（未成交）；PARTIALLY\_FILLED：部分成交；PARTIALLY\_CANCELED：部分撤销；FILLED：全部成交；CANCELED：已撤销；REJECTED：下单失败；EXPIRED：已过期
    | string | &nbsp; |

    | symbol | 交易对 | string | &nbsp; |

    | timeInForce | 有效类型 | string | &nbsp; |

    | triggerProfitPrice | 止盈触发价 | number(bigdecimal) | &nbsp; |

    | triggerStopPrice | 止损触发价 | number(bigdecimal) | &nbsp; |

    | returnCode | &nbsp; | integer(int32) | integer(int32) |


    &nbsp;
left_code_blocks:
    -
        code_block:
        title:
        language:
right_code_blocks:
    -
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"avgPrice\": 0,\n\t\t\"clientOrderId\": \"\",\n\t\t\"closePosition\": false,\n\t\t\"closeProfit\": 0,\n\t\t\"createdTime\": 0,\n\t\t\"executedQty\": 0,\n\t\t\"forceClose\": false,\n\t\t\"marginFrozen\": 0,\n\t\t\"orderId\": 0,\n\t\t\"orderSide\": \"\",\n\t\t\"orderType\": \"\",\n\t\t\"origQty\": 0,\n\t\t\"positionSide\": \"\",\n\t\t\"price\": 0,\n\t\t\"sourceId\": 0,\n\t\t\"state\": \"\",\n\t\t\"symbol\": \"\",\n\t\t\"timeInForce\": \"\",\n\t\t\"triggerProfitPrice\": 0,\n\t\t\"triggerStopPrice\": 0\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: javascript
---

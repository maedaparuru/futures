---
title: 根据profitId查询止盈止损
position_number: 10
type: get
split: '-------------------------------------'
description: |
    接口地址:/v1/entrust/profit-detail<br>
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

    | profitId | profitId | query | true | integer(int64) | &nbsp; |


    **响应状态**\:


    | 状态码 | 说明 | schema |

    | --- | --- | --- |

    | 200 | OK | CommonResponse&laquo;ProfitEntrustVO&raquo; |

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

    | result | &nbsp; | ProfitEntrustVO | ProfitEntrustVO |

    | createdTime | 时间 | integer(int64) | &nbsp; |

    | entryPrice | 开仓均价 | number(bigdecimal) | &nbsp; |

    | executedQty | 实际成交 | number(bigdecimal) | &nbsp; |

    | isolatedMargin | 逐仓保证金 | number(bigdecimal) | &nbsp; |

    | origQty | 数量（张） | number(bigdecimal) | &nbsp; |

    | positionSide | 仓位方向 | string | &nbsp; |

    | positionSize | 持仓数量（张） | number(bigdecimal) | &nbsp; |

    | positionType | 仓位类型 | string | &nbsp; |

    | profitId | 委托id | integer(int64) | &nbsp; |

    | state | 订单状态
    NOT\_TRIGGERED：新建委托（未触发）；TRIGGERING：触发中；TRIGGERED：已触发；USER\_REVOCATION：用户撤销；PLATFORM\_REVOCATION：平台撤销（拒绝）；EXPIRED：已过期
    | string | &nbsp; |

    | symbol | 交易对 | string | &nbsp; |

    | triggerPriceType | 触发价格类型：MARK\_PRICE(标记价格)；LATEST\_PRICE(最新价格) | string |
    &nbsp; |

    | triggerProfitPrice | 止盈价格 | number(bigdecimal) | &nbsp; |

    | triggerStopPrice | 止损价格 | number(bigdecimal) | &nbsp; |

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
        code_block: "{\n\t\"error\": {\n\t\t\"code\": \"\",\n\t\t\"msg\": \"\"\n\t},\n\t\"msgInfo\": \"\",\n\t\"result\": {\n\t\t\"createdTime\": 0,\n\t\t\"entryPrice\": 0,\n\t\t\"executedQty\": 0,\n\t\t\"isolatedMargin\": 0,\n\t\t\"origQty\": 0,\n\t\t\"positionSide\": \"\",\n\t\t\"positionSize\": 0,\n\t\t\"positionType\": \"\",\n\t\t\"profitId\": 0,\n\t\t\"state\": \"\",\n\t\t\"symbol\": \"\",\n\t\t\"triggerPriceType\": \"\",\n\t\t\"triggerProfitPrice\": 0,\n\t\t\"triggerStopPrice\": 0\n\t},\n\t\"returnCode\": 0\n}"
        title: Response
        language: javascript
---

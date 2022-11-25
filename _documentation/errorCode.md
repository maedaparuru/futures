---
title: response code
position_number: 9
parameters:
    -
        name:
content:
content_markdown: >-
    | httpStatus | description |

    | --- | --- |

    | 200 | The request is successful, please check the rc and mc sections
    further |

    | 404 | interface does not exist |

    | 429 | The request is too frequent, please control the request rate
    according to the speed limit requirement |

    | 500 | Service exception |

    | 502 | Gateway exception |

    | 503 | Service unavailable, please try again later |


    | rc | return Code |

    | --- | --- |

    | 0 | business success |

    | 1 | business failure |


    | mc | message code |

    | --- | --- |

    | SUCCESS | success |

    | FAILURE | fail |

    | AUTH\_001 | missing request header x-validate-appkey |

    | AUTH\_002 | missing request header x-validate-timestamp |

    | AUTH\_003 | missing request header x-validate-recvwindow |

    | AUTH\_004 | bad request header x-validate-recvwindow |

    | AUTH\_005 | missing request header x-validate-algorithms |

    | AUTH\_006 | bad request header x-validate-algorithms |

    | AUTH\_007 | missing request header x-validate-signature |

    | AUTH\_101 | ApiKey does not exist |

    | AUTH\_102 | ApiKey is not activated |

    | AUTH\_103 | Signature error |

    | AUTH\_104 | Unbound IP request |

    | AUTH\_105 | outdated message |

    | AUTH\_106 | Exceeded apikey permission |

    | SYMBOL\_001 | Symbol not exist |

    | SYMBOL\_002 | Symbol offline |

    | SYMBOL\_003 | Symbol suspend trading |

    | SYMBOL\_004 | Symbol country disallow trading |

    | ORDER\_001 | Platform rejection |

    | ORDER\_002 | insufficient funds |

    | ORDER\_003 | Trading Pair Suspended |

    | ORDER\_004 | no transaction |

    | ORDER\_005 | Order not exist |

    | ORDER\_006 | Too many open orders |

    | ORDER\_F0101 | Trigger Price Filter - Min |

    | ORDER\_F0102 | Trigger Price Filter - Max |

    | ORDER\_F0103 | Trigger Price Filter - Step Value |

    | ORDER\_F0201 | Trigger Quantity Filter - Min |

    | ORDER\_F0202 | Trigger Quantity Filter - Max |

    | ORDER\_F0203 | Trigger Quantity Filter - Step Value |

    | ORDER\_F0301 | Trigger QUOTE\_QTY Filter - Min Value |

    | ORDER\_F0401 | Trigger PROTECTION\_ONLINE Filter |

    | ORDER\_F0501 | Trigger PROTECTION\_LIMIT Filter |

    | ORDER\_F0601 | Trigger PROTECTION\_MARKET Filter |
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

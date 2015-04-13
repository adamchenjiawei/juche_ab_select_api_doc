# 删除话题 DeleteTopic

**POST**  /api/v1/users/delete_topic


##参数说明

| 参数 | 说明 |
| -- | -- |
| idfs | 看首页AB_Select_APP |
| secret | 看首页AB_Select_APP |
| access_token | AB用户的`access_token` |
| topic_id | 话题id |

##返回结果
| stauts | 说明 |
| -- | -- |
| 0 | 删除成功 |
| -1 | 传入参数不正确 |
| -2 | 传入参数不正确或者已经删除 |

{
  "status": 0,
  "data": "",
  "description": "删除成功"
}

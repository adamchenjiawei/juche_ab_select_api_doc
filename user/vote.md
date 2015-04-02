# 用户投票操作 Vote

**POST** /api/v1/users/add_vote

##参数说明

| 参数 | 说明 |
| -- | -- |
| idfs | 看首页AB_Select_APP |
| secret | 看首页AB_Select_APP |
| access_token | AB用户的`access_token` |
| topic_id | 话题ID |
| chooes_stauts | 投票状态 A／B |
| item_counts_a | a选项投票 |
| item_counts_b | b选项投票 |

`item_counts_a` and `item_counts_b`

当用户选择A时 `item_counts_a` 为 1 并且
                `item_counts_b` 为 0，反之亦然

##返回结果

| stauts | 说明 |
| -- | -- |
| 0 | 请求成功 |
| -1 | 传入参数有误 |
| -2 | 该用户已经投过票 |

```JSON
{
  status : 0,
  data:{
         id :"投票数id"
         topic_id: "话题id",
         item_counts_a:"A选项投票数",
         item_counts_b:"B选项投票数"
       },
  description : "OK"
}
```

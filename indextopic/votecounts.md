# 获取投票的数量 VoteCounts

**GET** `/api/v1/vote_counts/item_counts`

##参数说明
| 参数 | 说明 |
| -- | -- |
|topic_ids | 传入topic的id（例:1,2,4,5） |

##返回结果
| stauts | 说明 |
| -- | -- |
| 0 | 请求成功 |
| -1 | 获取投票数出错 |

```JSON
{
  status : 0,
  data:[
        {
        id: "投票数id",
        topic_id: "topic的id",
        item_counts_a :"选项A的票数",
        item_counts_b :"选项B的票数"
        }...
       ],
  description : "OK"
}```

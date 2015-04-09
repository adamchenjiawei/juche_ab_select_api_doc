# 发布话题 PublishTopic

**POST** /api/v1/topics/new_topic

##参数说明

| 参数 | 说明 |
| -- | -- |
| idfs | 看首页AB_Select_APP |
| secret | 看首页AB_Select_APP |
| access_token | AB用户的`access_token` |
| content | 话题内容 |
| chooes_a | 文字选项A |
| chooes_b | 文字选项B |
| chooes_img_a | 图片选项A |
| chooes_img_b | 图片选项B |

`4个选项参数只能有2个参数有值`

##返回结果

| stauts | 说明 |
| -- | -- |
| 0 | 发布成功 |
| -1 | 传入参数有误 |
| -2 | 发布失败 |

```JSON
{
  "status": 0,
  "data": {
    "topic_id": 21,
    "user_id": 16,
    "content": "asda",
    "chooes_a": "a",
    "chooes_b": "b",
    "chooes_img_a": "",
    "chooes_img_b": "",
    "time": "2015-04-08T11:31:14.953+08:00"
  },
  "description": "发布成功"
}

```


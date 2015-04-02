# 获取当前用户所发布的内容 UserTopic


**POST** /api/v1/users/user_topic

##参数说明

| 参数 | 说明 |
| -- | -- |
| idfs | 看首页AB_Select_APP |
| secret | 看首页AB_Select_APP |
| access_token | AB用户的`access_token` |
| page | 页码 |

##返回结果
| stauts | 说明 |
| -- | -- |
| 0 | 请求成功 |
| -1 | 参数出入有误 |
| -2 | 该用户当前未发布内容 |



```JSON
{
    status : "0",
    page : "页码",
    topic_total: "总共多少条数据",
    data : [
             {
              topic_id : "话题id",
              user_id  : "发布者的ID",
              content  : "话题的内容",
              chooes_a : "文字选项A",
              chooes_b : "文字选项B",
              chooes_img_a:"图片选项A",
              chooes_img_b:"图片选项B",
              time : "发布时间"
             }...
           ],
    description : "OK"
}
```

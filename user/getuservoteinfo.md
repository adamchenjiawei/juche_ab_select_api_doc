# 获取用户话题的投票信息  GetUserVoteInfo

**POST** /api/v1/users/vote_info

##参数说明

| 参数 | 说明 |
| -- | -- |
| idfs | 看首页AB_Select_APP |
| secret | 看首页AB_Select_APP |
| access_toen | AB用户的`access_token` |
| topic_ids | 话题id（例：1,2,3,4）|



##返回结果

| stauts | 说明 |
| -- | -- |
| 0 | 请求成功 |
| -1 | 传入参数有误 |


```JSON
{
 status : 0,
 total : "总共数据",
 data :[
        {topic_id : "话题id",
         chooes_status:"选择状态，返回A／B"
         }...
       ],
  escription : "OK"
}
```

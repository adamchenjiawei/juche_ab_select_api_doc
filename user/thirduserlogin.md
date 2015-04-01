# 第三方用户登录 ThirdUserLogin

**POST** /api/v1/users/oauth_login

##参数说明

| 参数 | 说明 |
| -- | -- |
| idfs | 看首页AB_Select_APP |
| secret | 看首页AB_Select_APP |
| uid | 第三方唯一id |
| provider |  第三方来源（例：weibo、qq..）|
| nick_name | 第三方获取的昵称 |
| portrait | 第三方的头像 |

#返回结果
| stauts | 说明 |
| -- | -- |
| 0 | 请求成功 |
| -1 | 传入参数有误 |

```JSON
{ status : "0",
  data:[
         {
          user_id: "用户ID",
          nick_name: "用户昵称",
          portrait: "用户头像",
          access_token : "用户的token",
          provider : "平台信息"
         },....
        ],
    description : "OK"
}
```

# 获取七牛凭证 Qiniu

**POST**  /api/v1/qiniu/uptoken

##参数说明

| 参数 | 说明 |
| -- | -- |
| idfs | 看首页AB_Select_APP |
| secret | 看首页AB_Select_APP |

##返回结果

```JSON
{
  "host": "域名",
  "ak": "密钥",
  "sk": "密钥",
  "bucket": "空间域",
  "ab_topic_dir": "路径"
}
```

# 获取最近时间话题

**GET** `/api/v1/topics/info`

##参数说明

| 参数 | 说明 |
| -- | -- |
| page | 页数 |


##返回结果
| stauts | 说明 |
| -- | -- |
| 0 | 请求成功 |
| -1 | 获取话题出错 |



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

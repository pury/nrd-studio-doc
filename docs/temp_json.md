# JSON文件

#### 配置

|   字段  | 类型 | 描述  |
|  ----  | ----  | ----  |
| title  | string | 项目名称 |

#### 节点

|   字段  | 类型 | 描述  |
|  ----  | ----  | ----  |
| id  | number| 索引 |
| name  | string | 名称 |
| image  | string | 图片（可选） |

#### 关系

|   字段  | 类型 | 描述  |
|  ----  | ----  | ----  |
| from  | number| 节点索引 |
| to  | number| 节点索引 |
| relation  | string | 关系名称 |



```
{
    "config": {
        "title": "demo示例"
    }, 
    "chart": {
        "nodes": [
            {
                "id": 0, 
                "name": "张三", 
                "image": "https://tech.pkoala.com/images/a.jpeg"
            }, 
            {
                "id": 1, 
                "name": "李四", 
                "image": "https://tech.pkoala.com/images/b.jpeg"
            }, 
            {
                "id": 2, 
                "name": "王五", 
                "image": "https://tech.pkoala.com/images/c.jpg"
            }
        ], 
        "links": [
            {
                "from": 0, 
                "to": 1, 
                "relation": "好友"
            }, 
            {
                "from": 0, 
                "to": 2, 
                "relation": "同学"
            }
        ]
    }
}
```
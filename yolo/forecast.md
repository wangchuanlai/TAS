# 图片预测(yoloObj:forecast)

## 对象方法

```lua
paddleYolo.forecast(图片对象)
```

<table><thead><tr><th>参数</th><th>类型</th><th width="108">必填</th><th>说明</th></tr></thead><tbody><tr><td>imgObj</td><td>userdata</td><td>是</td><td>需要检测的图片对象</td></tr></tbody></table>

## 返回值

| 返回值    | 类型    | 说明     |
| ------ | ----- | ------ |
| result | table | 返回检测结果 |

## 示例

```lua
---简单的示例
yoloObj = paddleYolo.init("/var/mobile/Media/yolo/lables.txt" ,"/var/mobile/Media/yolo/model.np")
--创建yolo 对象 在生产环境中 该操作会占用大量时间  通常使用全局变量 实例化一次就好
local result = yoloObj:forecast(screen.image())  -- 使用模型预测
print(result)                                    --打印结果


```

# 获取预测结果(yoloObj:result)

## 对象方法

```lua
yoloObj:result()
```

## 无参数

## 返回值

| 返回值    | 类型    | 说明    |
| ------ | ----- | ----- |
| result | table | 预测的结果 |

## 示例

```lua
--简单的示例
yoloObj = paddleYolo.init("/var/mobile/Media/yolo/lables.txt" ,"/var/mobile/Media/yolo/model.np")
--创建yolo 对象 在生产环境中 该操作会占用大量时间  通常使用全局变量 实例化一次就好
yoloObj:forecast(screen.image())  -- 使用模型预测
print(yoloObj:result())                                    --打印结果
```

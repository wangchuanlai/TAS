# 设置预测阈值(yoloObj:setThresh)

## 对象方法

```lua
yoloObj:setThresh(阈值)  -- 阈值范围 0.1 - 1.0
```

## 参数

| 参数     | 类型    | 必填 | 说明   |
| ------ | ----- | -- | ---- |
| thresh | float | 是  | 预测阈值 |

## 无返回值

## 示例

```lua
--简单的示例
yoloObj = paddleYolo.init("/var/mobile/Media/yolo/lables.txt" ,"/var/mobile/Media/yolo/model.np")
--创建yolo 对象 在生产环境中 该操作会占用大量时间  通常使用全局变量 实例化一次就好
yoloObj:setThresh(0.5)                                   --设置预测阈值 大于等于 0.5 的目标 
yoloObj:forecast(screen.image())  -- 使用模型预测
print(yoloObj:result())                                    --打印结果
local img = yoloObj:resultToImage()                        --获取图片结果
img:saveToAlbum()                                            --将图片保存的系统相册
```

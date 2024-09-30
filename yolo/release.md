# 手动释放(yoloObj:release)

## 对象方法

```lua
yoloObj:release()
```

## 无参数

## 无返回值

## 示例

```lua
--创建yolo 对象 该操作会占用大量时间  通常使用全局变量 实例化一次就好
yoloObj:setThresh(0.5)                                   --设置预测阈值 大于等于 0.5 的目标 
yoloObj:forecast(screen.image())  -- 使用模型预测
print(yoloObj:result())                                    --打印结果
local img = yoloObj:resultToImage()                        --获取图片结果
img:saveToAlbum()                                            --将图片保存的系统相册
yoloObj:release()                --手动释放掉yolo 对象 在生产环境中 劲量不要 频繁创建和释放对象 
```

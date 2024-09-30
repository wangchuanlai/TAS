# 隐藏(obj:hide())

## 函数

```lua
obj:hide()
```

## 无参数

## 返回值

| 返回值 | 类型       | 说明     |
| --- | -------- | ------ |
| obj | userdata | 屏幕绘制对象 |

## 示例

```lua
--在屏幕 100,200 的位置创建一个 宽度100 高度100的 屏幕绘制对象  
local sd = screenDraw.init(100,200,100,100)
sd:show()  --在屏幕上显示
sys.msleep(1000)
sd:hide()        --延迟1秒 影藏绘制
```

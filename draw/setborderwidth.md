# 设置边框的宽度(obj:setBorderWidth())

## 对象方法

```lua
obj:setBorderWidth(宽度)
```

## 参数

| 参数    | 类型     | 必填 | 说明   |
| ----- | ------ | -- | ---- |
| width | number | 是  | 边框宽度 |

## 返回值

| 返回值 | 类型       | 说明     |
| --- | -------- | ------ |
| obj | userdata | 屏幕绘制对象 |

## 示例

```lua
local sd = screenDraw.init(100,200,100,100)
sd:show():setTitle("随便起一个标题")   --显示出来 并设置 标题
sd:setTitleColor(0x00ff00)            --设置标题的颜色为蓝色
sd:setBorderWidth(3.0)                --设置边框的宽度
sys.msleep(1000)
```

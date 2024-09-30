# 设置边框的圆角(obj:setRadius())

## 对象方法

```lua
obj:setRadius(角度)
```

## 参数

| 参数     | 类型  | 必填 | 说明 |
| ------ | --- | -- | -- |
| radius | int | 是  | 角度 |

## 返回值

| 返回值 | 类型       | 说明     |
| --- | -------- | ------ |
| obj | userdata | 屏幕绘制对象 |

## 示例

```lua
local sd = screenDraw.init(100,200,100,100)
sd:show():setTitle("随便起一个标题")   --显示出来 并设置 标题
sd:setTitleColor(0x00ff00)            --设置标题的颜色为绿色
sd:setBorderWidth(3.0)                --设置边框的宽度
sd:setBorderColor(0x0000ff)            --设置边框颜色为蓝色
sd:setRadius(5)                        --设置边框圆角为5
sys.msleep(1000)    


---以下示例 将绘制一个圆形

local sd = screenDraw.init(100,100,200,200)
sd:show():setRadius(100 /4)   
sys.msleep(1000)


```

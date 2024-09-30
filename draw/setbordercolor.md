# 设置边框颜色(obj:setBorderColor())

## 对象方法

```lua
obj:setBorderColor(颜色值hex)
```

## 参数

| 参数    | 类型  | 必填 | 说明      |
| ----- | --- | -- | ------- |
| color | int | 是  | 16进制颜色值 |

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
sys.msleep(1000)
```

# 设置标题的颜色(obj:setTitleColor)

## 对象方法

```lua
obj:setTitleColor(颜色值hex)
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
--在屏幕 100,200 的位置创建一个 宽度100 高度100的 屏幕绘制对象  
local sd = screenDraw.init(100,200,100,100)
sd:show():setTitle("随便起一个标题")   --显示出来 并设置 标题
sd:setTitleColor(0x00ff00)            --设置标题的颜色为蓝色
sys.msleep(1000)
```

# 初始化 (screenDraw.init)

## 函数

```lua
screenDraw.init(坐标x, 坐标y, [宽度 ,高度 ,标题, 边框颜色, 边框宽度，标题字体大小, 标题颜色])
```

## 参数

| 参数          | 类型     | 必填 | 说明                |
| ----------- | ------ | -- | ----------------- |
| x           | int    | 是  | 横坐标               |
| y           | int    | 是  | 纵坐标               |
| w           | int    | 是  | 宽度                |
| h           | int    | 是  | 高度                |
| title       | string | 可选 | 标题 默认空字符串         |
| borderColor | int    | 可选 | 边框颜色 默认为 0xff0000 |
| borderWidth | number | 可选 | 边框宽度 默认 1.0       |
| fontSize    | number | 可选 | 字体大小 默认12         |
| titleColor  | int    | 可选 | 标题颜色 默认0xff0000   |

## 返回值

| 返回值 | 类型       | 说明     |
| --- | -------- | ------ |
| obj | userdata | 屏幕绘制对象 |

## 示例

```lua
--在屏幕 100,200 的位置创建一个 宽度100 高度100的 屏幕绘制对象 边框颜色为 绿色 标题颜色为 蓝色
local sd = screenDraw.init(100,200,100,100 ,"测试绘制" ,0x00ff00,2, 12, 0x0000ff)
sd:show()  --在屏幕上显示



```

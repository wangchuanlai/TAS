# 屏幕截图(screen.image)

## 函数

```lua
screen.image([x, y, x1, y1])
```

## 参数

| 参数 | 类型  | 必填 | 说明    |
| -- | --- | -- | ----- |
| x  | int | 可选 | 起始坐标x |
| y  | int | 可选 | 起始坐标y |
| x1 | int | 可选 | 结束坐标x |
| y1 | int | 可选 | 结束坐标y |

## 返回值

| 返回值    | 类型       | 说明   |
| ------ | -------- | ---- |
| imgObj | userdata | 图片对象 |

## 示例

```lua
local img = screen.image()        --全屏截图

local img = screen.image(100,100,200,200) --截取 屏幕坐标 100，200 图片

```

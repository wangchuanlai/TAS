# 获取某点的RGB值(screen.getColorRGB)

## 函数

```lua
screen.getColorRGB(坐标x, 坐标y)
```

## 参数

| 参数 | 类型  | 必填 | 说明    |
| -- | --- | -- | ----- |
| x  | int | 是  | 屏幕坐标x |
| y  | int | 是  | 屏幕坐标y |

## 返回值

| 返回值 | 类型  | 说明    |
| --- | --- | ----- |
| r   | int | 颜色值 R |
| g   | int | 颜色值 G |
| b   | int | 颜色值 B |

## 示例

```lua
local r, g, b = screen.getColorRGB(100,100) --获取坐标点 100,100 的 rgb 值
if r == 255 and g == 255 and 255 then
    print("颜色值 匹配")
end
```

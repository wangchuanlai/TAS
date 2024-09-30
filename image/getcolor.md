# 获取某点的颜色值(imgObj:getColor)

## 对象方法

```lua
imgObj:getColor(坐标x , 坐标y)
```

## 参数

| 参数 | 类型  | 必填 | 说明    |
| -- | --- | -- | ----- |
| x  | int | 是  | 屏幕坐标x |
| y  | int | 是  | 屏幕坐标y |

## 返回值

| 返回值   | 类型  | 说明          |
| ----- | --- | ----------- |
| color | int | 返回坐标位置的 颜色值 |

## 示例

```lua
local color = screen.image():getColor(100,100)  --获取屏幕位置 100,100 的颜色值
if color == 0xffffff then
    print("颜色值 匹配")
else
    print("颜色值 不匹配")
end
```

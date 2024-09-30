# 获取屏幕尺寸(screen.size)

## 函数

```lua
screen.size()
```

## 无参数

## 返回值

| 返回值    | 类型  | 说明   |
| ------ | --- | ---- |
| width  | int | 屏幕宽度 |
| height | int | 屏幕高度 |

## 示例

```lua
local width ,height = screen.size()
print(string.format("屏幕尺寸为:%d ,%d" ,width ,height))
```

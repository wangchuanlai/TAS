# 获取图片尺寸(imgObj:size)

## 对象方法

```lua
imgObj:size()
```

## 无参数

## 返回值

| 返回值    | 类型  | 说明   |
| ------ | --- | ---- |
| width  | int | 屏幕宽度 |
| height | int | 屏幕高度 |

## 示例

```lua
--简单的示例
local width ,height = screen.image():size()
print(string.format("图片的尺寸为:%d ,%d" ,width ,height))
```

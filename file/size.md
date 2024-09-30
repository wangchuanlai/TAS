# 获取文件的尺寸大小(file.size)

## 函数

```lua
file.size(文件路径)
```

## 参数

| 参数   | 类型     | 必填 | 说明   |
| ---- | ------ | -- | ---- |
| path | string | 是  | 文件路径 |

## 返回值

| 返回值  | 类型  | 说明   |
| ---- | --- | ---- |
| size | int | 文件大小 |

## 示例

```lua
print(string.format("图片文件的大小是：%d" ,file.size("/var/mobile/Media/1.png")))
```

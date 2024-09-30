# 获取某一行的内容(file.getLineText)

## 函数

```lua
file.getLineText(文件路径,行数)
```

## 参数

| 参数   | 类型     | 必填 | 说明   |
| ---- | ------ | -- | ---- |
| path | string | 是  | 文件路径 |
| line | int    | 是  | 行数   |

## 返回值

| 返回值  | 类型     | 说明  |
| ---- | ------ | --- |
| text | string | 行内容 |

## 示例

```lua
local text = file.getLineText("/var/mobile/Media/1.txt" , 1)  --获取txt文件中 第一行的内容
```

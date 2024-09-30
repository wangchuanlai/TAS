# 获取文件的总行数(file.lineCount)

## 函数

```lua
file.lineCount(文件路径)
```

## 参数

| 参数   | 类型     | 必填 | 说明   |
| ---- | ------ | -- | ---- |
| path | string | 是  | 文件路径 |

## 返回值

| 返回值   | 类型  | 说明    |
| ----- | --- | ----- |
| count | int | 文本总行数 |

## 示例

```lua
print(string.format("当前文件的总行数:%d" ,file.lineCount("/var/mobile/Media/1.txt")))
```

# 读取文件的所有内容(file.reads)

## 函数

```lua
file.reads(文件路径)
```

## 参数

| 参数   | 类型     | 必填 | 说明   |
| ---- | ------ | -- | ---- |
| path | string | 是  | 文件路径 |

## 返回值

| 返回值 | 类型     | 说明   |
| --- | ------ | ---- |
| res | string | 文件内容 |

## 示例

```lua
local fileText = file.reads("/var/mobile/Media/1.png")
```

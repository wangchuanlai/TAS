# 获取文件的多有行(file.getLines)

## 函数

```lua
file.getLines(文件路径)
```

## 参数

| 参数   | 类型     | 必填 | 说明   |
| ---- | ------ | -- | ---- |
| path | string | 是  | 文件路径 |

## 返回值

| 返回值    | 类型    | 说明       |
| ------ | ----- | -------- |
| result | table | 文件的所有行内容 |

## 示例

```lua
local result = file.getLines("/var/mobile/Media/1.txt")

for _,v in pairs(result) do
    print(string.format("第 %d 行内容:%s" ,_,v))
end
```

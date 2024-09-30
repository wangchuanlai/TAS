# 替换某一行的内容(file.resetLineText)

## 函数

```lua
file.resetLineText(文件路径,行数)
```

## 参数

| 参数   | 类型     | 必填 | 说明   |
| ---- | ------ | -- | ---- |
| path | string | 是  | 文件路径 |
| line | int    | 是  | 行数   |
| text | string | 是  | 新的内容 |

## 返回值

| 返回值 | 类型   | 说明     |
| --- | ---- | ------ |
| res | bool | 替换是否成功 |

## 示例

```lua
if file.resetLineText("/var/mobile/Media/1.txt" , 1 ,"新的内容") then
    print("替换成功")
end
```

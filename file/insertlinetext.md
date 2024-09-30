# 插入一行数据(file.insertLineText)

## 函数

```lua
file.insertLineText(文件路径, 行数，插入的内容)
```

## 参数

| 参数   | 类型     | 必填 | 说明      |
| ---- | ------ | -- | ------- |
| path | string | 是  | 文件路径    |
| line | int    | 是  | 需要插入的行数 |
| text | string | 是  | 需要插入的文本 |

## 返回值

| 返回值 | 类型   | 说明     |
| --- | ---- | ------ |
| res | bool | 操作是否成功 |

## 示例

```lua
if (file.insertLineText("/var/mobile/Media/1.txt" , 1 ,"需要插入的内容")) then
    print("插入成功")
end
```

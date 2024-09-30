# 写入数据到文件(file.writes)

## 函数

```lua
file.writes(文件路径,文本数据)
```

## 参数

| 参数   | 类型     | 必填 | 说明      |
| ---- | ------ | -- | ------- |
| path | string | 是  | 需要写入的路径 |
| text | string | 是  | 需要写入的数据 |

## 返回值

| 返回值 | 类型   | 说明     |
| --- | ---- | ------ |
| res | bool | 是否成功写入 |

## 示例

```lua
if (file.writes("/var/mobile/Media/1.txt" ,"随便写点数据进去")) then
    print("写入成功")
end
```

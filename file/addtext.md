# 追加写入数据(file.addText)(废弃)

## 函数

```lua
file.addText(文件路径,需要写入的文本)
```

## 参数

| 参数   | 类型     | 必填 | 说明      |
| ---- | ------ | -- | ------- |
| path | string | 是  | 文件路径    |
| text | string | 是  | 需要写入的文本 |

## 返回值

| 返回值 | 类型   | 说明     |
| --- | ---- | ------ |
| res | bool | 写入是否成功 |

## 示例

```lua
if (file.addText("/var/mobile/Media/1.txt" ,"随便写点数据进去")) then
    print("写入成功")
end
```

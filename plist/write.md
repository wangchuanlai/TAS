# 写plist内容(pilst.write)

## 函数

```lua
plist.write(文件路径,需要写入的table)
```

## 参数

| 参数   | 类型     | 必填 | 说明           |
| ---- | ------ | -- | ------------ |
| path | string | 是  | 文件路径         |
| tab  | table  | 是  | 需要写入的table数据 |

## 返回值

| 返回值 | 类型   | 说明     |
| --- | ---- | ------ |
| res | bool | 写入是否成功 |

## 示例

```lua
if plist.write("/var/mobile/Media/config.plist" ,{abc = "123"}) then
    print("写入成功")
end
```

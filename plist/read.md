# 读plist内容(plist.read)

## 函数

```lua
plit.read(文件路径)
```

## 参数

| 参数   | 类型     | 必填 | 说明        |
| ---- | ------ | -- | --------- |
| path | string | 是  | plist文件路径 |

## 返回值

| 返回值    | 类型    | 说明                |
| ------ | ----- | ----------------- |
| result | table | 成功返回table 失败返回nil |

## 示例

```lua
local result = plist.read("/var/mobile/Media/config.plist")
for k,v in pairs(result) do   --读取plist 文件 并遍历出来
    print(k ,v)
end
```

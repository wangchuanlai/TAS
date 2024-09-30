# 读剪贴板内容(pasteboard.read)

## 函数

```lua
pasteboard.read()
```

## 无参数

## 返回值

| 返回值  | 类型     | 说明               |
| ---- | ------ | ---------------- |
| text | string | 成功返回text 失败返回nil |

## 示例

```lua
local text = pasteboard.read()
if text then
    print(string.format("剪贴板的内容是:%s" ,text))
end
```

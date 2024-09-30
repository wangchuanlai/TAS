# 获取应用程序分组信息(app.groupInfo)

## 函数

```lua
app.groupInfo(应用唯一标识)
```

## 参数

| 参数                | 类型     | 必填 | 说明     |
| ----------------- | ------ | -- | ------ |
| bundle identifier | string | 是  | 应用唯一标识 |

## 返回值

| 返回值  | 类型    | 说明             |
| ---- | ----- | -------------- |
| info | table | 包含应用分组信息的table |

## 示例

```lua
local info = app.groupInfo("com.nssurge.inc.surge-ios")
print(info)
```

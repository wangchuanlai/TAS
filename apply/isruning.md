---
description: 仅支持越狱
hidden: true
---

# 应用程序是在否运行中(app.IsRauning   只支持越狱)

## 函数

```
app.isRuning(应用程序包名)
```

## 参数

| 参数                | 类型     | 必填 | 说明     |
| ----------------- | ------ | -- | ------ |
| bundle identifier | string | 是  | 应用唯一标识 |

## 返回值

| 返回值 | 类型   | 说明                   |
| --- | ---- | -------------------- |
| val | bool | 运行中返回true 否则返回 false |

## 示例

```lua
local res = app.isRuning("com.ss.iphone.ugc.aweme.lite")
if res then
    print("APP 正在运行中")
else
    print("APP 未运行")
end

```

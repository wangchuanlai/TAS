---
hidden: true
---

# 获取应用程序的process identifier(app.bidToPid 只支持越狱)

## 函数

```lua
app.bidToPid(应用唯一标识)
```

## 参数

| 参数                | 类型     | 必填 | 说明     |
| ----------------- | ------ | -- | ------ |
| bundle identifier | string | 是  | 应用唯一标识 |

## 返回值

| 返回值                | 类型  | 说明   |
| ------------------ | --- | ---- |
| process identifier | int | 进程id |

## 示例

```lua
print(string.format("应用的进程id:%d" ,app.bidToPid("com.ss.iphone.ugc.aweme.lite")))
```

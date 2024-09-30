---
hidden: true
---

# 获取前台应用bundle identifier(app.frontBid 只支持越狱)

## 函数

```
app.frontBid()
```

## 无参数

## 返回值

| 返回值               | 类型     | 说明     |
| ----------------- | ------ | ------ |
| bundle identifier | string | 应用唯一标识 |

## 示例

```lua
if app.frontBid() ~= "com.ss.iphone.ugc.aweme.lite" then
    app.run("com.ss.iphone.ugc.aweme.lite")
    sys.msleep(3000)
end
```

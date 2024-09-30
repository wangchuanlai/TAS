# 前台打开一个URL(app.openUrl)

## 函数

```lua
app.openUrl(url)
```

## 参数

| 参数  | 类型     | 必填 | 说明                                                                                                                                     |
| --- | ------ | -- | -------------------------------------------------------------------------------------------------------------------------------------- |
| url | string | 是  | URL 或 [URL Scheme](https://developer.apple.com/library/ios/featuredarticles/iPhoneURLScheme\_Reference/Introduction/Introduction.html) |

## 无返回值

## 示例

```lua
app.openUrl("http://www.baidu.com") -- 使用 Safari 打开百度

app.openUrl("prefs:root=General&path=ACCESSIBILITY") -- 跳转到 设置--通用--辅助功能
```

# 获取应用程序版本(app.version)

## 函数

```lua
app.version(应用唯一标识)
```

## 参数

| 参数                | 类型     | 必填 | 说明     |
| ----------------- | ------ | -- | ------ |
| bundle identifier | string | 是  | 应用唯一标识 |

## 返回值

| 返回值     | 类型     | 说明        |
| ------- | ------ | --------- |
| version | string | 应用程序的版本信息 |

## 示例

```lua

print(string.format("应用程序的版本：%s",app.version("com.ss.iphone.ugc.aweme.lite")))

```

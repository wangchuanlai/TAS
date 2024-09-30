# 获取应用程序安装路径(app.installPath)

## 函数

```lua
app.installPath(应用唯一标识)
```

## 参数

| 参数                | 类型     | 必填 | 说明     |
| ----------------- | ------ | -- | ------ |
| bundle identifier | string | 是  | 应用唯一标识 |

## 返回值

| 返回值 | 类型     | 说明     |
| --- | ------ | ------ |
| res | string | 应用安装路径 |

## 示例

```lua
print(string.format("应用的安装路径是:%s" ,app.installPath("com.ss.iphone.ugc.aweme.lite")))
```

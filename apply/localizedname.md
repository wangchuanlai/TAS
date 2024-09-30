# 获取应用程序本地化名称(app.localizedName)

## 函数

```lua
app.localizedName(应用唯一标识)
```

## 参数

| 参数                | 类型     | 必填 | 说明     |
| ----------------- | ------ | -- | ------ |
| bundle identifier | string | 是  | 应用唯一标识 |

## 返回值

| 返回值  | 类型     | 说明      |
| ---- | ------ | ------- |
| name | string | 应用本地化名称 |

## 示例

```lua

print(app.localizedName("com.ss.iphone.ugc.aweme.lite"))

```

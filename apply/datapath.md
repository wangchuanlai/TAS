# 获取应用程序沙盒路径(app.dataPath)

## 函数

```lua
app.dataPath(应用唯一标识)
```

## 参数

| 参数                | 类型     | 必填 | 说明     |
| ----------------- | ------ | -- | ------ |
| bundle identifier | string | 是  | 应用唯一标识 |

## 返回值

| 返回值  | 类型     | 说明     |
| ---- | ------ | ------ |
| path | string | 应用沙盒路径 |

## 示例

```lua

print(string.format("应用沙盒路径:%s" ,app.dataPath("com.apple.springboard")))

```

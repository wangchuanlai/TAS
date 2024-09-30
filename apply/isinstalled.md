# 应用程序是否安装(app.isInstalled)

## 函数

```lua
app.isInstalled(应用唯一标识)
```

## 参数

| 参数                | 类型     | 必填 | 说明     |
| ----------------- | ------ | -- | ------ |
| bundle identifier | string | 是  | 应用唯一标识 |

## 返回值

| 返回值 | 类型   | 说明                  |
| --- | ---- | ------------------- |
| res | bool | 已安装返回true 否则返回false |

## 示例

```lua
if app.isInstalled("com.ss.iphone.ugc.aweme.lite") then
    print("应用已安装")
else
    print("应用未安装")
end
```

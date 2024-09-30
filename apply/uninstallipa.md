# 卸载应用程序(app.uninstall)

## 函数

```lua
app.uninstall(应用唯一标识)
```

## 参数

<table><thead><tr><th width="193">参数</th><th>类型</th><th>必选</th><th>说明</th></tr></thead><tbody><tr><td>bundle identifier</td><td>string</td><td>是</td><td>应用唯一标识</td></tr></tbody></table>

## 返回值

| 返回值 | 类型   | 说明                 |
| --- | ---- | ------------------ |
| res | bool | 成功返回true 失败返回false |

## 示例

```lua
if app.uninstall("com.nssurge.inc.surge-ios") then
    print("卸载成功")
else
    print("卸载失败")
end
```

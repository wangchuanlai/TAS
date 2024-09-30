# 运行应用程序(app.run)

## 函数

```
app.run(应用程序包名)
```

| 参数                | 类型     | 必填 | 说明     |
| ----------------- | ------ | -- | ------ |
| bundle identifier | string | 是  | 应用唯一标识 |

## 返回值

| 返回值  | 类型   | 说明          |
| ---- | ---- | ----------- |
| flag | bool | 成功返回真 失败返回假 |

## 例子

```lua
local res = app.run("com.ss.iphone.ugc.aweme.lite")
sys.msleep(1000)
assert(res ,"app启动失败.")
```


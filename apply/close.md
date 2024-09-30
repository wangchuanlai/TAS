# 应用程序退出(app.close)

## 函数

```lua
app.close(应用程序包名 或 进程Id)
```

| 参数                 | 类型     | 必填 | 说明     |
| ------------------ | ------ | -- | ------ |
| bundle identifier  | string | 是  | 应用唯一标识 |
| process identifier | int    | 是  | 进程id   |

## 无返回值

## 例子

```lua
app.close("com.ss.iphone.ugc.aweme.lite")
```

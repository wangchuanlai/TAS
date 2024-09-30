---
hidden: true
---

# 获取前台应用的process identifier（只支持越狱）

## 函数

```lua
app.frontPid(应用唯一标识)
```

## 无参数

## 返回值

| 返回值                | 类型   | 说明   |
| ------------------ | ---- | ---- |
| process identifier | int  | 进程id |

## 示例

```lua
print(string.format("前台应用的进程id:%d" ,app.frontPid()))
```

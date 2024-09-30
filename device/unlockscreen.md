---
hidden: true
---

# 解锁屏幕(device.unlockScreen)(废弃)

## 函数

```lua
device.unlockScreen([解锁密码])
```

## 参数

| 参数       | 类型     | 必填 | 说明         |
| -------- | ------ | -- | ---------- |
| password | string | 可选 | 未设置密码 无需填写 |

## 无返回值

## 示例

```lua
if device.isScreenLocked() then   --屏幕锁定中 开始解锁屏幕
    device.unlockScreen()
    sys.msleep(1000)
end
```

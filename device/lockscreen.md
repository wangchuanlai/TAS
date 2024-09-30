---
hidden: true
---

# 锁定屏幕(device.lockScreen)(废弃)

## 函数

```lua
device.lockScreen()
```

## 无参数

## 无返回值

## 示例

```lua
device.lockScreen() --锁定屏幕
sys.msleep(1000)
if device.isScreenLocked() then
    print("屏幕已锁定")
end
```

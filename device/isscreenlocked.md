---
hidden: true
---

# 屏幕是否锁定(device.isScreenLocked)

## 函数

```lua
device.isScreenLocked()
```

## 无参数

## 返回值

| 返回值    | 类型   | 说明                  |
| ------ | ---- | ------------------- |
| result | bool | 锁定返回 true 否则返回false |

## 示例

```lua
if device.isScreenLocked() then
    print("屏幕处于锁定状态")
else
    print("屏幕已解锁")
end
```

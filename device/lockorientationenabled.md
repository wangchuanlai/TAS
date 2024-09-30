---
hidden: true
---

# 屏幕旋转是否开启(device.lockOrientationEnabled)(废弃)

## 函数

```lua
device.lockOrientationEnabled()
```

## 无参数

## 返回值

| 返回值    | 类型   | 说明                   |
| ------ | ---- | -------------------- |
| result | bool | 已启用返回 true 否则返回false |

## 示例

```lua
if device.lockOrientationEnabled() then
    print("锁定屏幕旋转已启用")
else
    print("锁定屏幕旋转未启用")
end
```

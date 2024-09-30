---
hidden: true
---

# 解锁屏幕旋转(device.unlockOrientation)(废弃)

## 函数

```lua
device.unlockOrientation()
```

## 无参数

## 无返回值

## 示例

```lua
if device.lockOrientationEnabled() then
    print("屏幕锁定 处于开启状态 关闭它")
    device.unlockOrientation()
end
```

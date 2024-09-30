---
hidden: true
---

# 锁定屏幕旋转(device.lockOrientation)(废弃)

## 函数

```lua
device.lockOrientation()
```

## 无参数

## 无返回值

## 示例

```lua
if not device.lockOrientationEnabled() then
    print("屏幕锁定 处于关闭状态 开启它")
    device.lockOrientation()
end
```

---
hidden: true
---

# 开打闪光灯(device.turnOnFlash)(废弃)

## 函数

```lua
device.turnOnFlash()
```

## 无参数

## 无返回值

## 示例

```lua
if not device.isFlashEnabled() then  
    print("闪光灯 未启用")
    device.turnOnFlash()  -- 打开闪光灯
end
```

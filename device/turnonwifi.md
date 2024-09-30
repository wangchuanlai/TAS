---
hidden: true
---

# 启用WIFI(device.turnOnWiFi)(废弃)

## 函数

```lua
device.turnOnWiFi()
```

## 无参数

## 无返回值

## 示例

```lua
if not device.isWiFiEnabled() then  
    print("wifi 未启用 启动它")
    device.turnOnWiFi()
end
```

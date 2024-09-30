---
hidden: true
---

# WiFi是否启用(device.isWiFiEnabled)(废弃)

## 函数

```lua
device.isWiFiEnabled()
```

## 无参数

## 返回值

| 返回值    | 类型   | 说明                   |
| ------ | ---- | -------------------- |
| result | bool | 已启用返回 true 否则返回false |

## 示例

```lua
if device.isWiFiEnabled() then
    print("wifi已启用")
else
    print("wifi未启用")
end
```

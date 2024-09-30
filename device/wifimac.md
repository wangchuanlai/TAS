# 获取设备的WiFi MAC(device.wifiMac)

## 函数

```lua
device.wifiMac()
```

## 无参数

## 返回值

| 返回值 | 类型     | 说明          |
| --- | ------ | ----------- |
| mac | string | wifi mac 地址 |

## 示例

```lua
print(string.format("当前设备的wifi MAC地址: %s" ,device.wifiMac()))
```

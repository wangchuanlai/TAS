# 获取设备蓝牙MAC(device.bluetoothMac)

## 函数

```lua
device.bluetoothMac()
```

## 无参数

## 返回值

| 返回值 | 类型     | 说明          |
| --- | ------ | ----------- |
| mac | string | wifi mac 地址 |

## 示例

```lua
print(string.format("当前设备蓝牙 MAC地址: %s" ,device.bluetoothMac()))
```

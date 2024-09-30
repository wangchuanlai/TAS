# 获取设备所有IP 信息(device.interIPAddres)

## 函数

```lua
device.interIPAddres()
```

## 无参数

## 返回值

| 返回值    | 类型    | 说明             |
| ------ | ----- | -------------- |
| result | table | 当前设备的 所有网卡IP地址 |

## 示例

```lua
print(device.interIPAddres())   --打印所有的网卡 Ip 信息
```

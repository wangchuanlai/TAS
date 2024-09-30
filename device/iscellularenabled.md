# 蜂窝网络是否启用(device.isCellularEnabled)

## 函数

```lua
device.isCellularEnabled()
```

## 无参数

## 返回值

| 返回值    | 类型   | 说明                   |
| ------ | ---- | -------------------- |
| result | bool | 已启用返回 true 否则返回false |

## 示例

```lua
if device.isCellularEnabled() then
    print("蜂窝网络已启用")
else
    print("蜂窝网络未启用")
end
```

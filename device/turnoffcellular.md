# 停用蜂窝网络(device.turnOffCellular)

## 函数

```lua
device.turnOffCellular()
```

## 无参数

## 无返回值

## 示例

```lua
if device.isCellularEnabled() then  
    print("wifi 已启用 ")
    device.turnOffCellular()   --停用蜂窝网络
end
```

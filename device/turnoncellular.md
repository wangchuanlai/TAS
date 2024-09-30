# 启用蜂窝网络(device.turnOnCellular)

## 函数

```lua
device.turnOnCellular()
```

## 无参数

## 无返回值

## 示例

```lua
if not device.isCellularEnabled() then  
    print("蜂窝网络 未启用")
    device.turnOnCellular()  --启用蜂窝网络
end
```

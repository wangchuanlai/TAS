# 获取当前背光亮度(device.backlightLevel)

## 函数

```lua
device.backlightLevel()
```

## 无参数

## 返回值

| 返回值   | 类型    | 说明     |
| ----- | ----- | ------ |
| level | float | 当前背光亮度 |

## 示例

```lua
local level = device.backlightLevel()
print(string.format("当前背光亮度:%f" ,level))
```

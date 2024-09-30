# 获取当前系统剩余内存(sys.availableMemory)

## 函数

```lua
sys.availableMemory()
```

## 无参数

## 返回值

| 返回值 | 类型     | 说明       |
| --- | ------ | -------- |
| val | number | 当前系统剩余内存 |

## 示例

```lua
print(string.format("当前系统未使用的内存：%f mb",sys.availableMemory()))
```

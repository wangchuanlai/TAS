# 获取当前进程使用的内存(sys.processUsedMemory)

## 函数

```lua
sys.processUsedMemory()
```

## 无参数

## 返回值

| 返回值 | 类型     | 说明        |
| --- | ------ | --------- |
| use | number | 已经使用的内存大小 |

## 示例

```lua
print(string.format("当前进程已经使用了：%f mb的内存",sys.processUsedMemory()))
```

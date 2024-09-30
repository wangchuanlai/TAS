# 获取系统已使用内存(sys.usedMemory)

## 函数

```lua
sys.usedMemory()
```

## 无参数

## 返回值

| 返回值 | 类型     | 说明        |
| --- | ------ | --------- |
| use | number | 当前系统使用内存量 |

## 示例

```lua
print(string.format("当前系统已经使用了：%f mb的内存",sys.usedMemory()))
```

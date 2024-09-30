# 当前VPN连接状态(vpn.connectState)

## 函数

```lua
vpn.connectState()
```

## 无参数

## 返回值

| 返回值   | 类型     | 说明     |
| ----- | ------ | ------ |
| state | string | 当前连接状态 |

## 示例

```lua
print(string.format("当前VPN 连接状态是: %s" ,vpn.connectState()))
```

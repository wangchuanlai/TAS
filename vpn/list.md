---
hidden: true
---

# 获取所有VPN(vpn.list)(废弃)

## 函数

```lua
vpn.list()
```

## 无参数

## 返回值

| 返回值    | 类型    | 说明         |
| ------ | ----- | ---------- |
| result | table | 返回所有VPN 信息 |

## 示例

```lua
for k ,v in pairs(vpn.list()) do    ---遍历所有VPN 信息
    print(v.name , v.udid) 
end
```

# 选中VPN(vpn.select)

## 函数

```lua
vpn.select(vpn名称)
```

## 参数

| 参数   | 类型     | 必填 | 说明         |
| ---- | ------ | -- | ---------- |
| name | string | 是  | 需要删除的vpn名称 |

## 返回值

| 返回值    | 类型   | 说明                 |
| ------ | ---- | ------------------ |
| result | bool | 成功返回true 失败返回false |

## 示例

```lua
vpn.select("随便起个名字")   --选中VPN
```

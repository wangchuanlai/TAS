---
hidden: true
---

# 闪光灯是否启用(device.isFlashEnabled)(废弃)

## 函数

```lua
device.isFlashEnabled()
```

## 无参数

## 返回值

| 返回值    | 类型   | 说明                   |
| ------ | ---- | -------------------- |
| result | bool | 已启用返回 true 否则返回false |

## 示例

```lua
if device.isFlashEnabled() then
    print("闪光灯已打开")
else
    print("闪光灯已关闭")
end
```

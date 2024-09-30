---
hidden: true
---

# 设置背光亮度(device.setBacklightLevel)(废弃)

## 函数

```lua
device.setBacklightLevel(亮度)
```

## 参数

<table><thead><tr><th width="117">参数</th><th width="85">类型</th><th width="72">必填</th><th>说明</th></tr></thead><tbody><tr><td>level</td><td>float</td><td>是</td><td>参数必须在 0.0- 1.0之间</td></tr></tbody></table>

## 无返回值

## 示例

```lua
device.setBacklightLevel(1.0)  --设置最大亮度
device.setBacklightLevel(0.0)  --设置最小亮度
```

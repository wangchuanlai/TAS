---
hidden: true
---

# 设置音量(device.setVolume)(废弃)

## 函数

```lua
device.setVolume(音量)
```

## 参数

<table><thead><tr><th width="139">参数</th><th width="124">类型</th><th width="87">必填</th><th>说明</th></tr></thead><tbody><tr><td>volume</td><td>float</td><td>是</td><td>参数必须在 0.0 - 1.0 之间</td></tr></tbody></table>

## 无返回值

## 示例

```lua
device.setVolume(1)  -- 设置最大音量
device.setVolume(0)  -- 设置静音
```

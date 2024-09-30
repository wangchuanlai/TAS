---
hidden: true
---

# 当前屏幕旋转方向(device.screenOrientation)(废弃)

## 函数

```lua
device.screenOrientation()
```

## 无参数

## 返回值

| 返回值  | 类型  | 说明   |
| ---- | --- | ---- |
| init | int | 屏幕方向 |

## 示例

```lua
local screenInit = device.screenOrientation()
if screenInit == 0 then
    print("home 在下")
elseif screenInit == 1 then
    print("home键在右")
elseif screenInit == 2 then
    print("home键在左")
end
```

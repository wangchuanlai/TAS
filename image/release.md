# 手动释放图片对象(imgObj:release)

## 函数

```lua
imgObj:release()
```

## 无参数

## 无返回值

## 示例

```lua
--简单的示例  通常情况下 我们不需要手动释放  lua的垃圾回收机制会自动回收
local img = screen.image()    --屏幕截图 
img:release()

--以下示例 频繁调用的情况下 需要手动释放 （lua 5.4 除外）
while true do
    local img = screen.image()            --产生图片对象
    img:release()                            --释放图片对象
end

--释放的图片对象的 另一种方式 （lua 5.4 除外）
while true do
    local img = screen.image()            --产生图片对象
    collectgarbage("collect")                --执行一次垃圾回收
end

--在lua5.4 下 垃圾回收速度非常快  无需要 手动释放 
while true do
    local img = screen.image()            --产生图片对象
end


```

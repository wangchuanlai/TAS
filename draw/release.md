# 手动释放(obj:release)

## 函数

```lua
obj:release()
```

## 无参数

## 无返回值

## 示例

```lua
--在屏幕 100,200 的位置创建一个 宽度100 高度100的 屏幕绘制对象  
local sd = screenDraw.init(100,200,100,100)
sd:show()  --在屏幕上显示
sd:release()            --手动销毁对象 立即释放内存
```

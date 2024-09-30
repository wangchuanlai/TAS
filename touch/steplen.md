# 触摸移动步长(obj:stepLen)

## 函数

```lua
obj:stepLen(每次移动步长)
```

## 参数

| 参数  | 类型  | 必填 | 说明      |
| --- | --- | -- | ------- |
| len | int | 是  | 每次移动的步长 |

## 返回值

| 返回值 | 类型       | 说明       |
| --- | -------- | -------- |
| obj | userdata | touch 对象 |

## 示例

```lua
local t = touch.down(100,100 ) --手指按下
t:stepLen(10)        --设置每次移动 10个像素点
t:stepDelay(5)        --每次滑动等待
t:move(200,200)        --手指移动到 200-200的位置
t:up()    --手指抬起

--链式调用示例
touch.down(100,100):stepLen(10):stepDelay(5):move(200,200):up()    --和上方示例 同样的效果
```

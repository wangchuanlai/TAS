# 触摸等待(obj: await)

## 函数

```lua
obj:await(等待时间)
```

## 参数

| 参数    | 类型  | 必填 | 说明       |
| ----- | --- | -- | -------- |
| sleep | int | 是  | 等待时间 毫秒级 |

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
t:await(500)         --延迟等待 500毫秒后抬起手指
t:up()    --手指抬起

--链式调用示例
touch.down(100,100):stepLen(10):stepDelay(5):move(200,200):await(500):up()    --和上方示例 同样的效果
```

# 触摸移动每步延迟(obj:stepDelay)

## 函数

```lua
obj:stepDelay(每步延迟)
```

## 参数

<table><thead><tr><th>参数</th><th>类型</th><th width="105">必填</th><th>说明</th></tr></thead><tbody><tr><td>delay</td><td>int</td><td>是</td><td>每滑动一步 等待的时间</td></tr><tr><td></td><td></td><td></td><td></td></tr><tr><td></td><td></td><td></td><td></td></tr></tbody></table>

## 返回值

| 返回值 | 类型       | 说明       |
| --- | -------- | -------- |
| obj | userdata | touch 对象 |
|     |          |          |
|     |          |          |

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

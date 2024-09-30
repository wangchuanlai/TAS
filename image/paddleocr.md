# 对图片文字识别(imgObj:paddleOcr)

## 对象方法

```lua
imgObj:paddleOcr([x, y, x1, y1])
```

## 参数

| 参数 | 类型  | 必填 | 说明    |
| -- | --- | -- | ----- |
| x  | int | 可选 | 起始坐标x |
| y  | int | 可选 | 起始坐标y |
| x1 | int | 可选 | 结束坐标x |
| y1 | int | 可选 | 结束坐标y |

## 返回值

| 返回值    | 类型    | 说明     |
| ------ | ----- | ------ |
| result | table | 返回识别结果 |

## 示例

```lua
--简单的示例
local result = screen.image():paddleOcr()        --全屏识别
print("识别结果" , result)

local result = screen.image(100,100,200,200):paddleOcr()    --范围识别
print("识别结果",result)
```

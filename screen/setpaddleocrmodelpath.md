# 设置paddleOcr模型路径(screen.setPaddleOcrModelPath)

## 函数

```lua
screen.setPaddleOcrModelPath(model存放路径)
```

## 参数

| 参数   | 类型     | 必填 | 说明            |
| ---- | ------ | -- | ------------- |
| path | string | 是  | paddle 模型存放路径 |

## 无返回值

## 示例

```lua
--简单的示例,如果有更好的模型，一般情况下直接使用内置的visionOcr 或 paddleOcr即可
screen.setPaddleOcrModelPath("/var/mobile/Media/paddleModel")
```


# 初始化模型(paddleYolo.init)

## 函数

```lua
paddleYolo.init(标签文件路径,模型文件路径)
```

<table><thead><tr><th>参数</th><th>类型</th><th width="108">必填</th><th>说明</th></tr></thead><tbody><tr><td>labelPath</td><td>string</td><td>是</td><td>模型对应的标签文件</td></tr><tr><td>modelPath</td><td>string</td><td>是</td><td>模型文件</td></tr><tr><td>thresh</td><td>float</td><td>可选</td><td>预测相似度 默认 0.5 (0.1-1.0)</td></tr><tr><td>inputWidth</td><td>int</td><td>可选</td><td>模型 input 宽度 默认 608</td></tr><tr><td>inputHeight</td><td>int</td><td>可选</td><td>模型 input 高度 默认 608</td></tr></tbody></table>

## 返回值

| 返回值     | 类型       | 说明            |
| ------- | -------- | ------------- |
| yoloObj | userData | 返回yolo 的实例话对象 |

## 示例

```lua
---简单的示例
yoloObj = paddleYolo.init("/var/mobile/Media/yolo/lables.txt" ,"/var/mobile/Media/yolo/model.np")
--创建yolo 对象 在生产环境中 该操作会占用大量时间  通常使用全局变量 实例化一次就好
yoloObj:forecast(screen.image())  -- 使用模型预测


```

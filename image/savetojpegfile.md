# 保存图片到JPG文件(imgObj:saveToJpegFile)

## 对象方法

```lua
imgObj:saveToJpegFile(保存路径)
```

## 参数

| 参数   | 类型     | 必填 | 说明     |
| ---- | ------ | -- | ------ |
| path | string | 是  | 图片保存路径 |

## 返回值

<table><thead><tr><th>返回值</th><th width="135.33333333333331">类型</th><th>说明</th></tr></thead><tbody><tr><td>bool</td><td>bool</td><td>保存成功返回 true 否则返回 false</td></tr></tbody></table>

## 示例

```lua
--简单的示例
screen.image():saveToJpegFile("/var/mobile/Media/test.png")  --截图并保存到PNG文件

```

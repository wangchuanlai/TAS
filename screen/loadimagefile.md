# 从文件加载图片对象(screen.loadImageFile)

## 函数

```lua
screen.loadImageFile(图片文件路径)
```

## 参数

| 参数   | 类型     | 必填 | 说明      |
| ---- | ------ | -- | ------- |
| path | string | 是  | 图片的存储路径 |

## 返回值

| 返回值    | 类型       | 说明     |
| ------ | -------- | ------ |
| imgObj | userdata | 返回图片对象 |

## 示例

```lua
--简单的示例
local imgObj = screen.loadImageFile("/var/mobile/Media/test.png")
if imgObj then
    imgObj:saveToAlbum()        --将图片对象 保存到系统相册
end
```

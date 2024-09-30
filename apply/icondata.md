# 获取应用程序icon图标数据(app.iconData)

## 函数

```lua
app.iconData(应用唯一标识)
```

## 参数

| 参数                | 类型     | 必填 | 说明     |
| ----------------- | ------ | -- | ------ |
| bundle identifier | string | 是  | 应用唯一标识 |

## 返回值

| 返回值       | 类型     | 说明         |
| --------- | ------ | ---------- |
| imageData | string | 应用图标的PNG数据 |

## 示例

```lua
local imgData = app.iconData("com.ss.iphone.ugc.aweme.lite")   --获取app的图片数据
if imgData then
    screen.loadImageData(imgData):saveToAlbum()                --把图片保存到系统相册
end
```

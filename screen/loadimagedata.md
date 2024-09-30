# 从数据加载图片对象(screen.loadImageData)

## 函数

```lua
screen.loadImageData(图片数据)
```

## 参数

| 参数        | 类型     | 必填 | 说明   |
| --------- | ------ | -- | ---- |
| imageData | string | 是  | 图片数据 |

## 返回值

| 返回值    | 类型       | 说明     |
| ------ | -------- | ------ |
| imgObj | userdata | 返回图片对象 |

## 示例

```lua
--简单的示例
local code ,header, body = http.get("https://www.baidu.com/img/PCtm_d9c8750bed0b3c7d089fa7d55720d6cf.png")
if code == 200 then
    local imgObj = screen.loadImageData(body)
    if imgObj then
        imgObj:saveToAlbum()        --将图片对象 保存到系统相册
    end
end
```

# opencv 图片二值化(imgObj:cvBinarization)

## 函数

```lua
imgObj:cvBinarization([阈值])
```

## 参数

| 参数        | 类型  | 必填 | 说明      |
| --------- | --- | -- | ------- |
| threshold | int | 可选 | 默认值 128 |

## 返回值

| 返回值    | 类型       | 说明     |
| ------ | -------- | ------ |
| imgObj | userdata | 新的图片对象 |

## 示例

```lua
--简单的示例
local img = screen.image()    --屏幕截图 
local newImg = img:cvBinarization()            --二值化图片
newImg:saveToAlbum()                    --保存到系统相册


local img = screen.image(100,100,200,200)    --屏幕截图 
local newImg = img:cvBinarization(180)            --二值化图片 并设置阈值为 180
newImg:saveToAlbum()                    --保存到系统相册
```

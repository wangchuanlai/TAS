# 图片二值化(imgObj:binarization)

## 函数

```lua
imgObj:binarization(色偏数组)
```

## 参数

| 参数     | 类型             | 必填 | 说明   |
| ------ | -------------- | -- | ---- |
| colors | table 或 string | 可选 | 色偏信息 |

## 返回值

| 返回值    | 类型       | 说明     |
| ------ | -------- | ------ |
| imgObj | userdata | 新的图片对象 |

## 示例

```lua
--简单的示例
local img = screen.image()    --屏幕截图 
local newImg = img:binarization({
    {0x23a82e , 0x202020},                    --设置 0x23a82e 颜色值的 色偏 0x202020
    {0xfffe0a , 0x202020},                     --设置 0xfffe0a 颜色值的 色偏 0x202020
})            --二值化图片
newImg:saveToAlbum()                    --保存到系统相册

--以下示例 产生的结果 和上面示例 产生的结果完全一样
local img = screen.image()                    --屏幕截图 
local newImg = img:binarization("23a82e-202020;fffe0a-202020")            --二值化图片
newImg:saveToAlbum()                        --保存到系统相册
```

# 在图片中找图(imgObj:findImage)

## 对象方法

```lua
imgObj:findImage(图片对象,[x, y, x1, y1])
```

## 参数

<table><thead><tr><th>参数</th><th>类型</th><th width="113">必填</th><th>说明</th></tr></thead><tbody><tr><td>imgObj</td><td>userdata</td><td>是</td><td>图片对象</td></tr><tr><td>x</td><td>int</td><td>可选</td><td>起始坐标x</td></tr><tr><td>y</td><td>int</td><td>可选</td><td>起始坐标y</td></tr><tr><td>x1</td><td>int</td><td>可选</td><td>结束坐标x</td></tr><tr><td>y1</td><td>int</td><td>可选</td><td>结束坐标y</td></tr></tbody></table>

## 返回值

| 返回值 | 类型  | 说明               |
| --- | --- | ---------------- |
| x   | int | 成功返回坐标x  否则返回 -1 |
| y   | int | 成功返回坐标y  否则返回 -1 |

## 示例

```lua
--简单的示例 从屏幕创建图片对象
local imgObj = screen.image()            --全屏截图

local img = screen.image(100,100,200,200) --随便截个图 用来测试找图
local x ,y = imgObj:findImage(img)         --全屏找图
if x ~= -1 and y ~= -1 then
    print(string.format("成功找到图片拉坐标: x= %d, y= %d" ,x ,y))
end

--另一个示例 从图片文件加载图片对象 
local x ,y = imgObj:findImage(screen.loadImageFile("/var/mobile/Media/test.png"))--全屏找图
if x ~= -1 and y ~= -1 then
    print(string.format("成功找到图片拉坐标: x= %d, y= %d" ,x ,y))
end


--另一个示例 从图片文件加载图片对象 
local x ,y = imgObj:findImage(screen.loadImageFile("/var/mobile/Media/test.png") ,
100,100,400,600 )        --范围找图
if x ~= -1 and y ~= -1 then
    print(string.format("成功找到图片拉坐标: x= %d, y= %d" ,x ,y))
end

```

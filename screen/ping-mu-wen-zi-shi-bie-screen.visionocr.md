# 屏幕文字识别(screen.visionOcr)

## 函数

```lua
screen.visionOcr([x, y, x1, y1])
```

## 参数

<table><thead><tr><th width="173">参数</th><th>类型</th><th>必填</th><th>说明</th></tr></thead><tbody><tr><td>x</td><td>int</td><td>可选</td><td>起始坐标x</td></tr><tr><td>y</td><td>int</td><td>可选</td><td>起始坐标y</td></tr><tr><td>x1</td><td>int</td><td>可选</td><td>结束坐标x</td></tr><tr><td>y1</td><td>int</td><td>可选</td><td>结束坐标y</td></tr></tbody></table>

## 返回值

| 返回值    | 类型    | 说明     |
| ------ | ----- | ------ |
| result | table | 返回识别结果 |

## 示例

```lua
--简单的示例
local result = screen.visionOcr()        --全屏识别
print("识别结果" , result)

local result = screen.visionOcr(100,100,200,200)    --范围识别
print("识别结果",result)


local img = screen.image()  --全屏二值化识别
local newImg = img:binarization("0x1D2746-0x505050")  
local result = newImg:visionOcr()
print("全屏二值化识别结果",result)

local img = screen.image(100,100,200,200)  --范围二值化识别
local newImg = img:binarization("0x1D2746-0x505050")  
local result = newImg:visionOcr()
print("范围二值化识别结果",result)

```

```lua
--所有识别的内容连成一句返回结果
--函数用来转义字符串中的特殊字符，确保模式匹配时不出错
function escape_lua_pattern(s)
    local pattern_characters = {"%", ".", "(", ")", "[", "]", "+", "-", "*", "?"}
    for i = 1, #pattern_characters do
        local c = pattern_characters[i]
        s = string.gsub(s, "%" .. c, "")
    end
    return s
end
local result = screen.visionOcr()       
str=""
for k, v in pairs(result) do
	str = str.. v.text
end
print("原始 : ",str)
print("去掉特殊字符 : ",escape_lua_pattern(str))

```

<pre class="language-lua"><code class="lang-lua"><strong>--全屏识别并圈起来
</strong><strong>local result = screen.visionOcr()   --也可以screen.visionOcr(100,100,200,200)
</strong>print(result)
local tab = {}
for k,v in pairs(result) do
    local drawView = screenDraw.init( math.ceil( v.x ),math.ceil( v.y ),math.ceil( v.w ), math.ceil( v.h ), v.string ,0x00ff00 , 1.0 , 12, 0x00ff00)
    table.insert(tab, drawView)
    drawView:show()
end
sys.msleep(1000*10)
</code></pre>



**注意事项 效果不佳可以测试paddleOcr()**

{% content-ref url="paddleocr.md" %}
[paddleocr.md](paddleocr.md)
{% endcontent-ref %}

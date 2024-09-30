# 屏幕多点找色(screen.findColors)

## 函数

```lua
screen.findColors(颜色值数组,[相似度 或色偏值] ,[是否匹配多个目标] ,[始坐标x]
,[开始坐标y] ,[结束坐标x] ,[结束坐标y])
```

## 参数

<table><thead><tr><th width="167">参数</th><th width="121">类型</th><th width="134">必填</th><th>说明</th></tr></thead><tbody><tr><td>colors</td><td>table</td><td>是</td><td>颜色值数组</td></tr><tr><td>similar</td><td>int</td><td>可选</td><td>相似度 或 色偏值（默认 相似度 95）</td></tr><tr><td>findAll</td><td>string</td><td>可选</td><td>是否匹配多个目标（默认 false）</td></tr><tr><td>x</td><td>int</td><td>可选</td><td>起始坐标x (默认 0)</td></tr><tr><td>y</td><td>int</td><td>可选</td><td>起始坐标y (默认 0)</td></tr><tr><td>x1</td><td>int</td><td>可选</td><td>结束坐标x (默认 屏幕宽度)</td></tr><tr><td>y1</td><td>int </td><td>可选</td><td>结束坐标y (默认 屏幕高度)</td></tr></tbody></table>

## 返回值

| 返回值      | 类型    | 说明                  |
| -------- | ----- | ------------------- |
| x        | int   | 成功返回坐标 失败返回 -1      |
| y        | int   | 成功返回坐标 失败返回 -1      |
| multiple | table | 当模式为匹配多个结果时 使用此类返回值 |

## 示例

```lua
---简单的示例    相似度模式
local x, y = screen.findColors({
    {  123,  177, 0x030712 },
    {  157,   96, 0xFD6303 },
    {  242,  196, 0x062C50 },
    {  126,  211, 0x011D32 },
    {   47,  138, 0x1C395B },
    {   80,  112, 0x092D4D },
} ,95)
if (x ~= -1 and y ~= -1) then
    print(string.format("成功找到坐标 x = %d ，y = %d" , x ,y))
end


---简单的示例    色偏模式
local x, y = screen.findColors({
    {  123,  177, 0x030712 },
    {  157,   96, 0xFD6303 },
    {  242,  196, 0x062C50 },
    {  126,  211, 0x011D32 },
    {   47,  138, 0x1C395B },
    {   80,  112, 0x092D4D },
} ,0x202020)
if (x ~= -1 and y ~= -1) then
    print(string.format("成功找到坐标 x = %d ，y = %d" , x ,y))
end


---简单的示例    
local x, y = screen.findColors({
    {  123,  177, 0x030712 , 80 },    --设置这个点的 相似度为 80
    {  157,   96, 0xFD6303 , 0x202020},        --设置这个点的色偏模式
    {  242,  196, 0x062C50 },                --以下使用色偏模式 值为 0x202020
    {  126,  211, 0x011D32 },
    {   47,  138, 0x1C395B },
    {   80,  112, 0x092D4D },
} ,0x202020)
if (x ~= -1 and y ~= -1) then
    print(string.format("成功找到坐标 x = %d ，y = %d" , x ,y))
end


---简单的示例    
local x, y = screen.findColors({
    {  123,  177, 0x030712 , 80 },    --设置这个点的 相似度为 80
    {  157,   96, 0xFD6303 , 0x202020},        --设置这个点的色偏模式
    {  242,  196, 0x062C50 },                --以下使用色偏模式 值为 0x202020
    {  126,  211, 0x011D32 },
    {   47,  138, 0x1C395B },
    {   80,  112, 0x092D4D },
} ,0x202020 , 100,100,300,300)            --设置多点找色区域为 起始点 100,100 结束点 300,300
if (x ~= -1 and y ~= -1) then
    print(string.format("成功找到坐标 x = %d ，y = %d" , x ,y))
end


---简单的示例 匹配多个结果
local result = screen.findColors({
    {  123,  177, 0x030712 , 80 },    --设置这个点的 相似度为 80
    {  157,   96, 0xFD6303 , 0x202020},        --设置这个点的色偏模式
    {  242,  196, 0x062C50 },                --以下使用色偏模式 值为 0x202020
    {  126,  211, 0x011D32 },
    {   47,  138, 0x1C395B },
    {   80,  112, 0x092D4D },
} ,0x202020 , "find_all" ,100,100,300,300)            --设置多点找色区域为 起始点 100,100 结束点 300,300

for k ,v in pairs(result) do
    print(string.format("第 %d 个结果 x = %d, y = %d" ,k ,v[1] ,v[2]))
end
```


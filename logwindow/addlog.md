# 在窗口上添加日志(obj:addLog)

## 对象方法

```lua
obj:addLog(日志文本, [文本颜色，文字大小])
```

## 参数

<table><thead><tr><th>参数</th><th>类型</th><th width="116">必填</th><th>说明</th></tr></thead><tbody><tr><td>logString</td><td>string</td><td>是</td><td>要显示的日志文本</td></tr><tr><td>logColor</td><td>int</td><td>可选</td><td>文本显示的颜色(限本条)</td></tr><tr><td>StringSize</td><td>float</td><td>可选</td><td>文本显示的大小 (限本条)</td></tr></tbody></table>

## 无返回值

## 示例

```lua
---简单的封装
function print(log)
    if (not LW) then
        --创建一个日志显示窗口  背景颜色为黑色 透明度为 0.3 日志颜色为 绿色  字体大小为18
        LW = logWindow.init(100,100 ,500,35 ,0.3,0x000000 ,0x00ff00, 18)  
    end
    LW:addLog(log)
end


print("显示一个 日志")
sys.msleep(1000)        --延迟一些时间 避免被 lua的垃圾回收机制 回收掉
--你将会看到 屏幕显示出了
```

# 模拟输入(key.sendText)

## 函数

```lua
key.sendText(字符串)  --
```

## 参数

<table><thead><tr><th>参数</th><th>类型</th><th width="83">必填</th><th>说明</th></tr></thead><tbody><tr><td>str</td><td>string</td><td>是</td><td>入的字符串 注意 只支持 英文，数字  符号 </td></tr><tr><td>msleep</td><td>int</td><td>可选</td><td>每输入一个字符的延迟时间 默认20毫秒</td></tr></tbody></table>

## 无返回值

## 示例

```lua
key.sendText("www.baidu.com" , 20) --模拟输入百度网站
```



**注意事项  此函数不符合要求，可以尝试inputText()**&#x20;

{% content-ref url="inputtext.md" %}
[inputtext.md](inputtext.md)
{% endcontent-ref %}

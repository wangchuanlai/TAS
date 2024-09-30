---
description: 该函数 触犯法律 现已废弃
hidden: true
---

# 模拟输入文字(key.inputText)

## 函数

```lua
key.inputText(需要输入的文字)
```

## 参数

| 参数   | 类型     | 必填 | 说明      |
| ---- | ------ | -- | ------- |
| text | string | 是  | 需要输入的文字 |

## 无返回值

## 示例

```lua

key.inputText("你好")    --模拟输入文字

key.inputText("\b")                --删除一个字符

for i = 1, 10 do                    --删除10个字符
    key.inputText("\b")
end

```

**注意事项  此函数不符合要求，可以尝试sendText()**

{% content-ref url="../key/sendtext.md" %}
[sendtext.md](../key/sendtext.md)
{% endcontent-ref %}


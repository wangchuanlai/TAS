# 随机生成字符串(string.random)

## 函数

```lua
string.random(字符串 ,随机几个字符）
```

## 参数

| 参数  | 类型     | 必填 | 说明        |
| --- | ------ | -- | --------- |
| str | string | 是  | 待处理的字符串   |
| len | int    | 是  | 需要随机字符的个数 |

## 返回值

| 返回值 | 类型     | 说明     |
| --- | ------ | ------ |
| res | string | 处理过的文本 |

## 示例

```lua
string.random("随便写点字abcddadadada" ,10)  --从字符串中 随机10个字符
```

# JSON解码(json.decode)

## 函数

```lua
json.decode(json字符串)
```

## 参数

| 参数      | 类型     | 必填 | 说明          |
| ------- | ------ | -- | ----------- |
| jsonStr | string | 是  | 待转换的json字符串 |

## 返回值

| 返回值 | 类型    | 说明              |
| --- | ----- | --------------- |
| tab | table | 标准的lua table 数组 |

## 示例

```lua

local tab = json.decode('{"abc":"测试字符串", "bcd": 1 }')
print(tab)

```

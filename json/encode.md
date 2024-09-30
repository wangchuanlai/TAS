# JSON编码(json.encode)

## 函数

```lua
json.encode(数组)
```

## 参数

| 参数  | 类型    | 必填 | 说明           |
| --- | ----- | -- | ------------ |
| tab | table | 是  | 待转成json格式的数组 |

## 返回值

| 返回值     | 类型     | 说明      |
| ------- | ------ | ------- |
| jsonStr | string | json字符串 |

## 示例

```lua
local jsonStr = json.encode({
    abc = "测试字符串",
    bcd = 1,
})
```

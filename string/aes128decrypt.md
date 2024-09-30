# aes128解密(string.aes128Decrypt)

## 函数

```lua
string.aes128Decrypt(字符串 ,密钥)
```

## 参数

| 参数  | 类型     | 必填 | 说明      |
| --- | ------ | -- | ------- |
| str | string | 是  | 待处理的字符串 |
| key | string | 是  | 加密密钥    |

## 返回值

| 返回值 | 类型     | 说明     |
| --- | ------ | ------ |
| res | string | 处理过的文本 |

## 示例

```lua
string.aes128Encrypt("随便写点字" ,"1234567890abcdef"):aes128Decrypt("1234567890abcdef")
```

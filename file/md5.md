# 获取文件md5(file.md5)

## 函数

```lua
file.md5(文件路径)
```

## 参数

| 参数   | 类型     | 必填 | 说明   |
| ---- | ------ | -- | ---- |
| path | string | 是  | 文件路径 |

## 返回值

| 返回值 | 类型     | 说明      |
| --- | ------ | ------- |
| md5 | string | 文件的md5值 |

## 示例

```lua
print(file.md5("/var/mobile/Media/1.txt"))
```

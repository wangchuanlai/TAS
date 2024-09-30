# 判断文件是否存在(file.existe)

## 函数

```lua
file.existe(path)
```

## 参数

| 参数   | 类型     | 必填 | 说明   |
| ---- | ------ | -- | ---- |
| path | string | 是  | 文件路径 |

## 返回值

| 返回值 | 类型   | 说明                   |
| --- | ---- | -------------------- |
| res | bool | 文件存在返回true 否则返回false |

## 示例

```lua
if (file.existe("/var/mobile/Media/1.png")) then
    print("文件存在")
else
    print("图片文件不存在")
end
```

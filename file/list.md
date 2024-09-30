# 遍历文件夹(file.list)

## 函数

```lua
file.list(路径)
```

## 参数

| 参数   | 类型     | 必填 | 说明    |
| ---- | ------ | -- | ----- |
| path | string | 是  | 文件夹路径 |

## 返回值

| 返回值  | 类型    | 说明        |
| ---- | ----- | --------- |
| list | table | 文件夹下所有文件名 |

## 示例

```lua
local fileList = file.list("/var/mobile/Media")

for k,v in pairs(fileList) do        --遍历文件
    print(v)
end
```

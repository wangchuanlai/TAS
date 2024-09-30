# 安装应用程序(app.installIpa)

## 函数

```lua
app.installIpa(ipa文件存放路径 ,回调函数)
```

## 参数

| 参数       | 类型       | 必填 | 说明        |
| -------- | -------- | -- | --------- |
| path     | string   | 是  | ipa文件存放路径 |
| callback | function | 可选 | 回调函数      |

## 回调函数参数

| 参数       | 类型  | 说明      |
| -------- | --- | ------- |
| progress | int | ipa安装进度 |

## 返回值

| 返回值 | 类型   | 说明                 |
| --- | ---- | ------------------ |
| res | bool | 成功返回true 失败返回false |

## 示例

```lua

--简单的示例
if app.installIpa("/var/mobile/Media/surge.ipa") then
    print("安装成功")
else
    print("安装失败")
end


--带回调函数的示例
local result = app.installIpa("/var/mobile/Media/surge.ipa" , function(progress) 
    print(string.format("当前安装进度:%d" ,progress))
end)
if result then
    print("安装成功")
else
    print("安装失败")
end

```

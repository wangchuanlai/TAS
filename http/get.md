# 发送GET请求(http.get)

## 函数

```lua
http.get(URL地址, [超时时间]， [请求头])
```

## 参数

| 参数      | 类型     | 必填 | 说明          |
| ------- | ------ | -- | ----------- |
| url     | string | 是  | url地址       |
| timeOut | int    | 可选 | 超时时间 默认 60秒 |
| header  | table  | 可选 | 请求头         |

## 返回值

| 返回值    | 类型     | 说明     |
| ------ | ------ | ------ |
| code   | int    | 请求状态码  |
| header | table  | 请求头部信息 |
| body   | string | 网页内容   |

## 示例

```lua
local code, header, body = http.get("https://www.baidu.com" , 30 ,{
    ["User-Agent"] = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.36"
})

if code == 200 then
    print(header)                    --打印头部信息
    print(body)                      --打印网页内容
end

```

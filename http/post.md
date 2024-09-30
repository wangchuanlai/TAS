# 发送POST请求(http.post)

## 函数

```lua
http.post(Url, [超时时间]，[请求头], [发送数据])
```

## 参数

| 参数      | 类型     | 必填 | 说明      |
| ------- | ------ | -- | ------- |
| url     | string | 是  | 网址      |
| timeOut | int    | 可选 | 超时时间    |
| header  | table  | 可选 | 请求头     |
| data    | string | 可选 | 需要发送的数据 |

## 返回值

| 返回值    | 类型     | 说明     |
| ------ | ------ | ------ |
| code   | int    | 请求状态码  |
| header | table  | 请求头部信息 |
| body   | string | 返回数据   |

## 示例

```lua
local code, header, body = http.post("https://www.baidu.com" , 30 ,{
    ["User-Agent"] = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.36"
} ,"username=1237489&password=237348")

if code == 200 then
    print(header)                    --打印头部信息
    print(body)                      --打印网页内容
end
```

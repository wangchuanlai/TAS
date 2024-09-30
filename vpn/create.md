# 创建VPN(vpn.create)

## 函数

```lua
vpn.create(名称,vpn服务器 , vpn用户名, vpn密码, vpn密钥 ,[类型])
```

## 参数

<table><thead><tr><th width="145">参数</th><th width="107">类型</th><th width="75">必填</th><th>说明</th></tr></thead><tbody><tr><td>name</td><td>string</td><td>是</td><td>vpn显示的名称</td></tr><tr><td>server</td><td>string</td><td>是</td><td>服务器地址</td></tr><tr><td>username</td><td>string</td><td>是</td><td>vpn用户名</td></tr><tr><td>password</td><td>string</td><td>是</td><td>vpn密码</td></tr><tr><td>key</td><td>string</td><td>是</td><td>vpn密钥</td></tr><tr><td>type</td><td>number</td><td>可选</td><td>参数为1时 l2tp类型 否则 IPsec  默认1</td></tr></tbody></table>

## 返回值

| 返回值     | 类型   | 说明              |
| ------- | ---- | --------------- |
| result  | bool | 成功返回 true 失败返回假 |

## 示例

```lua
if vpn.create("随便起个名字","192.168.100.2" , "username", "password", "suibianzhenggemimayo" ,1 ) then
    print("创建VPN 成功")
end
```

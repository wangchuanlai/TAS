# 打码



下载  [https://wwfp.lanzouv.com/ix3zg2aq3gmf\
](https://wwfp.lanzouv.com/ix3zg2aq3gmf) 也可以加群通过群文件下载

<pre class="language-lua"><code class="lang-lua"><strong>打码文件FengWan.tas文件放在 /var/mobile/Media/svip/lua
</strong></code></pre>



```lua
fengwan = require("FengWan")
fw = fengwan.init("FEFGG66244|BXMCKDIFMNWWRFG","6001")--密码串与题型


screen.image(371,131,966,365):saveToPngFile("/var/mobile/Media/svip/lua/yz.png") 
local result, tid = fw:uploadImg(screen.loadImageFile("/var/mobile/Media/svip/lua/yz.png"))

if result then
print("请求成功 tid =" ,tid)
	for i=1,60 do
		result ,msg = fw:getResult(tid)
		print(result ,msg)
		sys.msleep(1000)
		if result then
			break
		end
	end
else
	print(result)
    print("请求失败 原因 =",tid)
	return  false
end

```



打码官网[https://feng.suanst.com/](https://feng.suanst.com/)    &#x20;

密码串可在官网个人中心中看到



需要更多功能，可以参考[https://www.showdoc.com.cn/fengwan/10259124040432367](https://www.showdoc.com.cn/fengwan/10259124040432367)


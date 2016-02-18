
#CTFGAME_week1

--------
过了week1感觉需要多看书了，还有不会python的话会很惨。

##WEB从0开始之PHP代码审计0 

考查php弱类型，通过传入$array来绕过函数的检验null。 我是看[这篇文章](http://drops.wooyun.org/tips/4483)学到的
构造成 `?name[]=1&password[]=3`的样子即可得到flag

![](http://7xr0ty.com1.z0.glb.clouddn.com/10.PNG)

##密码学从0开始之1.1 

打开之后F12发现有个注释里全是二进制，一开始以为是7bit ASCII 或者是 8bit ASCII。后来发现是png图片

![](http://7xr0ty.com1.z0.glb.clouddn.com/11.PNG)
这个工具`字符信息与二进制` 百度一下可以下到
还需要用到一个16进制编辑器`winhex` 百度同样可以下到
复制一下16进制数里的内容 
在winhex新建一个文件 鼠标右键->编辑->剪贴板数据->写入->选择`ASCII Hex` 
另存为到 `你找得到的位置` 然后对其重命名为XXX.png 
然后打开它...

![](http://7xr0ty.com1.z0.glb.clouddn.com/12.PNG)


##MISC从0开始之流量分析1

下载下来丢进wireshark
然后File->Export Objects->HTTP
发现有个名为flag的文件选中它之后然后save as  找到那个文件对其重命名为"xxx.rar" 解压完还是得到一个名为flag的文件用winhex打开得到flag
(感觉我的做题过程略显诡异与麻烦）
![](http://7xr0ty.com1.z0.glb.clouddn.com/13.PNG)

##密码学从0开始之1

点横之类的感觉是摩斯电码 百度一下在线摩斯电码解密 

##MISC从0开始之编码1

base全家桶 不会python有不会python的[办法](http://pbaseconverter.com/)
先用base16转一下，base32转不了？别着急 删掉等号再转base32 最后转base64 得flag
base32是个坑 
![](http://7xr0ty.com1.z0.glb.clouddn.com/14.PNG)

##lightless&aklis的渗透教室-2 

如图发送post请求

![](http://7xr0ty.com1.z0.glb.clouddn.com/15.PNG)

得到响应 咦 不在这

![](http://7xr0ty.com1.z0.glb.clouddn.com/16.PNG)

找一下原始数据

![](http://7xr0ty.com1.z0.glb.clouddn.com/17.PNG)


##MISC 驾驶技术科目一 

还是丢到wireshark里
然后File->Export Objects->HTTP
好像是浏览记录有很多图片文本啥的 
莫名的出现了个奇怪的cad1.php还是来自ak老司机
![](http://7xr0ty.com1.z0.glb.clouddn.com/18.PNG)
下下来看看是啥
![](http://7xr0ty.com1.z0.glb.clouddn.com/19.PNG)
是个base64 解码一下得到flag


##MISC 驾驶技术科目二

科目一里的flag的{}里面还是base64解一下得到科目二的入口

得到ak老司机的支付宝图片 
另存为到本地之后
###朋友，你混贴吧吗？你听说过[图种](http://baike.baidu.com/view/7114230.htm)吗？
把后缀改为.zip `不是rar`
解压得到二维码 扫之得flag


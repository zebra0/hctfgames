# CTFGAME-week0

------

 说起来week0的感想大概是：

> * 用好google
##WEB从0开始之0.2
由提示得出要伪造一个cookie，用fiddler伪造如下cookie
![](http://7xr0ty.com1.z0.glb.clouddn.com/%E6%8D%95%E8%8E%B73.PNG)
显然
![](http://7xr0ty.com1.z0.glb.clouddn.com/%E6%8D%95%E8%8E%B74.PNG)

##MISC从0开始之流量分析0
 一个pcap文件用wireshark打开搜索含有flag的响应
 ![](http://7xr0ty.com1.z0.glb.clouddn.com/%E6%8D%95%E8%8E%B75.PNG)

## MISC从0开始之Steganography0
网页打开发现是一张图片另存为之后直接丢`notepad++`
![](http://7xr0ty.com1.z0.glb.clouddn.com/%E6%8D%95%E8%8E%B76.PNG)

##step0
下个断点跑一下就好
![](hhttp://7xr0ty.com1.z0.glb.clouddn.com/%E6%8D%95%E8%8E%B77.PNG)

##CTF coding step0
一开始以为要手工后来被提示要用管道Ubuntu下一行代码  `echo "A/n" | nc 115.29.77.78 9999`

##lightless的渗透教室-1
一开始想偏了 对http理解还是太肤浅 后来想到两个请求可以包含在一个请求中

![](http://7xr0ty.com1.z0.glb.clouddn.com/8.PNG)

##WEB从0开始之0.1	
印象中是抓了个302包 然后http头部有flag 


##WEB从0开始之0

隐藏的很隐蔽 在MISC下的一条js响应中

![](http://7xr0ty.com1.z0.glb.clouddn.com/9.PNG)

##MISC从0开始之编码0

base64

##密码学从0开始之0

凯撒密码 然后根据hctf的位置推算一下偏移量 得flag

# CTFGAME-week0

------

 说起来week0的感想大概是：

> * 用好google
##WEB从0开始之0.2
由提示得出要伪造一个cookie，用fiddler伪造如下cookie
![](http://a.picphotos.baidu.com/album/s%3D1600%3Bq%3D90/sign=1112149a3cc79f3d8be1e0368a91f660/0df3d7ca7bcb0a462a30da5c6c63f6246b60af41.jpg)
显然
![](http://e.picphotos.baidu.com/album/s%3D1600%3Bq%3D90/sign=479d9fb8ac64034f0bcdc6009ff34240/77094b36acaf2eddafaa188c8a1001e93901937f.jpg)

##MISC从0开始之流量分析0
 一个pcap文件用wireshark打开搜索含有flag的响应
 ![](http://f.picphotos.baidu.com/album/s%3D1600%3Bq%3D90/sign=6fdb46268cd4b31cf43c90bdb7e61c0e/f2deb48f8c5494eed529527c2af5e0fe99257e4f.jpg)

## MISC从0开始之Steganography0
网页打开发现是一张图片另存为之后直接丢`notepad++`
![](http://f.picphotos.baidu.com/album/s%3D1600%3Bq%3D90/sign=b1bc4361339b033b2888f8dc25fe0da2/0ff41bd5ad6eddc4344cea9e3edbb6fd5266332f.jpg)

##step0
下个断点跑一下就好
![](http://g.picphotos.baidu.com/album/s%3D1600%3Bq%3D90/sign=e8e20636f1246b607f0eb672dbc8213d/4610b912c8fcc3ce951691569545d688d53f2084.jpg)

##CTF coding step0
一开始以为要手工后来被提示要用管道Ubuntu下一行代码  `echo "A/n" | nc 115.29.77.78 9999`

##lightless的渗透教室-1
一开始想偏了 对http理解还是太肤浅 后来想到两个请求可以包含在一个请求中

![](http://f.picphotos.baidu.com/album/s%3D1600%3Bq%3D90/sign=a2e2ca6d9c504fc2a65fb403d5eddc60/4b90f603738da977b4dec04eb751f8198718e3e6.jpg)

##WEB从0开始之0.1	
印象中是抓了个302包 然后http头部有flag 


##WEB从0开始之0

隐藏的很隐蔽 在MISC下的一条js响应中

![](http://a.picphotos.baidu.com/album/s%3D1600%3Bq%3D90/sign=4952ea079f22720e7fcee6fc4bfb3137/c83d70cf3bc79f3db879ab55bda1cd11728b293e.jpg)

##MISC从0开始之编码0

base64

##密码学从0开始之0

凯撒密码 然后根据hctf的位置推算一下偏移量 得flag

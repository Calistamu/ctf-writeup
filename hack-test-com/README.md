# 关于hack-test.com的游戏攻略
[hack-test.com---一个有意思的网站](http://www.hack-test.com/index.htm)
## Level 1
由javascript代码得到答案是:null
![](images/1.png)
[第一次不知所措，有搜索](https://www.cnblogs.com/tk091/archive/2012/09/26/2703593.html)
## Level 2
弹出了一个窗口，填入password:l3l
![](images/2.png)
## Level 3
![](images/3.png)
## Level 4
做了好久，突然发现，之前都是在本关弹出弹框，而第四关的弹框是网页跳转，直接跳到第五关
![](images/4-1.png)
![](images/4.png)
## Level 5
![](images/5.jpg)
## Level 6
![](images/6.png)
## Level 7
这次不是在源代码中，找了很久
![](images/7-1.png)
差点没找到
![](images/7-2.png)
提交后
![](images/7-3.png)
回到第七关，看到提示
![](images/8.png)
明明输入正确，但是还是错为什么呢？我发现我的页面和别的小伙伴页面不一样，我之前用的IE和chrome浏览器，我自己也觉得为什么排版这么难看。然后看到IE和chrome的控制台都有报错。
[浏览器兼容](https://blog.csdn.net/weixin_30672019/article/details/96213889)
![](images/7-4.png)
## Level 8
查看源代码
![](images/8-1.png)
查看pwd2.php
![](images/8-2.jpg)
根据提示访问'http://www.hackertest.net/images/phat.gif',右下角看到
![](images/8-3.png)  
提示找Photoshop文件,由于pdd和psd是photoshop特有的图像格式，访问"http://www.hackertest.net/images/phat.pdd"，404报错说明没有，'http://www.hackertest.net/images/phat.gif'，弹出弹窗，保存图片。
photoshop打开，删去图层，得到账号和密码。  
![](images/8-4.jpg)
## Level 9
查看源代码，还是尝试访问'http://www.hackertest.net/images/phat.gif',发现是之前的页面，不知道怎么破。
但是level8没有下拉框，level9下拉，看到如下
![](images/9-1.png)
因此base64 decode得到：'gazebruh'，并加在网页最后,加上'.php'，进入第十关。
## Level 10
![](images/10-2.jpg)
看到多了一行字，而这些字长得和其他的有细微差别。
![](images/10-1.png)
从源代码中得到：shackithalf，输入后发现网页加载就像是有问题，一开始还以为是网不好。
![](images/10-3.jpg)
查看源代码
![](images/10-4.png)
进入下一关
## Level 11
尝试images/try.gif，没有线索，上方显示如下，进入下一关。
![](images/11-1.png)
## Level 12
线索
![](images/12-1.png)
这一次只有一个图片
![](images/12-2.png)
## Level 13
首页就给了提示
![](images/13-1.png)
## Level 14
![](images/14-1.png)
这一次图片没有水印，但是发现totally.php可能可以，尝试后通过
## Level 15 && Level 16
提示查看图片，但是打开是这样
![](images/15-1.png)
另存为后打开  
![](images/15-2.png)  
notepad打开  
![](images/15-3.png)
网页打开  
![](images/15-4.png)  
根据提示
![](images/15-5.png)
还是无法正常打开，另存为，Notepad打开
![](images/15-6.png)  
不是单纯的曾经，以前是在主页后加xx.php,这一次排列组合'/unaviable'和'/images'和'Ducky.php'，得到'http://www.hackertest.net/unavailable/Ducky.php'
## Level 17
得到提示
![](images/17-1.png)
打开cmd查看ip
![](images/17-2.jpg)
发现Ip不一样,因为火狐有代理，以相同浏览器的为准。[内网ip和外网ip](https://blog.csdn.net/Alexwym/article/details/81772446)
![](images/17-3.png)
提示回退上一层，输入网址  
![](images/17-4.png)
## Level 18
尝试'images/n00b.gif'没有线索,在看代码，好像真的需要cookie，但是发现了线索，尝试成功
![](images/18-1.png)
## Level 19
![](images/19-1.png)
根据代码给的提示打开图片
![](images/19-2.png)
## Level 20
给出提示,应该可以得到一个域名
![](images/20-1.png)
base64 decode得到的结果再解码，最后出现  
![](images/20-2.png)  
访问'www.streetkorner.net/gb22332'不对,访问'http://www.hackertest.net/gb22332/'
![](images/20-3.png)
HTTP版本不受支持,但是这个错误像是提前做好的错误  
![](images/20-4.png)
想了好久看到提示说使用错误文件，访问'http://www.hackertest.net/gb22332/505'，状态404，不对,访问'http://www.hackertest.net/505'状态200，对了。
![](images/20-5.png)
访问'http://www.hackertest.net/403',状态404.访问'http://www.hackertest.net/505/403'
![](images/20-6.png)  
好懵啊，一搜索，42？!,访问'http://www.hackertest.net/42.php' 
* 《银河系漫游指南》  
 
![](images/20-7.png)  
点击
![](images/20-8.png)
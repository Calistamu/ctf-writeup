# Web
## Web前置技能
### HTTP协议
#### 请求方式
##### 题目
![](images/httprequest.png)
##### 题解
参考[win10配置curl](https://www.jianshu.com/p/cc9cf0e3966e)，看到配置成功页面
![](images/curl-ok.png)
[curl 的用法指南-阮一峰的网络日志](http://www.ruanyifeng.com/blog/2019/09/curl-reference.html)根据题目提示更改Http请求，得到flag.  
![](images/httprequest-flag.png)
#### 302跳转
##### 题目
![](images/http302.png)
##### 题解
* 分析：  
网页打开  
![](images/http302-1.png)  
![](images/http302-2.png)  
使用bp抓包，找到目标包然后send into repeater  
![](images/http302-3.png) 

GO以后结果如下
![](images/http302-flag.png)
#### Cookie
##### 题目
![](images/httpcookie.png)
##### 题解
* 由于Bp一直没能抓到正确的包，抓到的包都没有cookie这一栏  
![](images/httocookie-1.png)

使用curl  
![](images/httocookie-flag.png)
#### 基础认证
##### 题目
##### 题解
#### 响应包源代码
##### 题目
##### 题解
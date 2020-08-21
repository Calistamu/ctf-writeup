# ctf-writeup
## 集锦
[CTF-Site](https://github.com/myndtt/CTF-Site)
[awesome-ctf](https://github.com/apsdehal/awesome-ctf)
### actual-combat --- 自己的实战wp
- [x] 腾讯犀牛鸟t-star-2020.6.30
* t-star的wp没有保存，一共十道题做出一道，是sql联合查询的题。
- [x] 第十三届全国大学生信息安全竞赛-2020.8.21
* 一共22道，做出一道Crypto。Web还太差，平时无脑题膨胀我。pwn和reverse第一次碰。misc有一道是要用windows写字板打开就能看到竖着的flag。

### [ctfhub](https://www.ctfhub.com/#/index)
>wp目录：ctfhub

竞赛模式：Jeopardy-解题、AwD-攻防模式、RHG-自动化[ AI自动化]、RW-真实世界、KoH-抢占山头、Mix[混合]

题目类型：Web、Pwn、Reverse、Crypto、Misc

* 通常来说Pwn类题目给出的远程服务器信息为`nc IP_ADDRESS PORT`，例如`nc4567`这种形式，表示在`1.2.3.4`这个IP的`4567`端口上运行了该题目

* Misc常见的题型有图片隐写、视频隐写、文档隐写、流量分析、协议分析、游戏、IoT相关等等。五花八门，种类繁多。
#### 工具配置
##### Web
##### Misc
###### 数据隐写类
- [x] 010Edior
- [x] Stegsolve
###### 流量分析类
- [x] Wireshark
###### 电子取证类
- [x] volatility(KALI自带)
###### 物联网类
- [] QEMU
- [] Binwalk
###### 密码破解类
- [] HashCat
- [] EWSA
- [] 在线网站
### [攻防世界](https://adworld.xctf.org.cn/)
>wp目录：xctf

### [i春秋](https://www.ichunqiu.com/)

### [ctf-wiki](https://github.com/ctf-wiki/ctf-wiki)
```
# deployed locally, with the following steps:
# 1. clone
git clone https://github.com/ctf-wiki/ctf-wiki.git
# 2. requirements
pip install -r requirements.txt
# generate static file in site/
mkdocs build
# deploy at http://127.0.0.1:8000
mkdocs serve
```
### [黑吧闯关之古墓密探](http://hkyx.myhack58.com/)
- []已通关
>wp目录：myhack58
### [黑客丛林之旅](http://www.fj543.com/hack/)
- [] 已通关
### [hack-test.com](http://www.hack-test.com/index.htm)
- [x] 已通关
>wp目录：hack-test-com
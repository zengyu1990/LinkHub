#关于
所谓的LinkHub就是一个链接聚合器。 

当你在网上看到某些有趣的链接不知道在哪里分享的时候，就可以分享到这里，让更多的人看到它。

地址 [linkhub.sinaapp.com](http://linkhub.sinaapp.com)

#功能&特色
在功能和一些细节上参考了两个我非常喜欢的站：hacker news和V2EX。主要有以下几点：

##金钱系统
我们使用金钱系统限制用户的发言次数。在一定程度上保证网站内容的质量。这应该是V2EX的特色之一。

金钱系统的内容有：
```
用户首次注册时，会有附送20个金币。
每发送一个链接，消耗2个金币。
链接被删除，消耗2个金币。
每天签到会收获4个金币
收获评论得到1个金币
发送评论消耗1个金币
链接评论被删除，消耗1个金币。
```

##书签
在页面的底部有个Add Link（书签）的链接，在chrome或者firefox浏览器下将该链接拖至书签栏，即可自动生成一个书签。

用法就是：
  1.  停留在想要提交的页面
  2.  点击AddLink书签，即可跳转到LinkHub的submit页面，此时页面已自动填写好相关信息。
  3.  点击提交按钮。（建议用户对生成的信息做相应修改后再提交）

##结点
结点功能是出于对不同链接分类而增加的。

使用场景是这样的：

对于一个设计人员来说，可能希望看到与设计相关的链接，并且不想被程序代码相关的链接所打扰。提交的链接也极可能是与设计相关的。

所以当用户选择了某个结点，则网站将默认提供相关的链接给用户，除非用户选择更换结点。提交的链接也默认属于该结点，除非用户手动更改。

##热度排名
关于最热排名的算法，参考了hacker news的算法。简单但是有效，使用python只用需要一句就可以实现。

具体见：[Link](http://www.ruanyifeng.com/blog/2012/02/ranking_algorithm_hacker_news.html)

##RSS
暂时只能订阅最新发布的列表。

##收藏
收藏自己认为有用的链接。方便以后查阅。

在首页，登陆状态下，鼠标移动到链接左侧序号处，会出现收藏按钮。点击即可收藏。或者在评论页，标题右侧的收藏按钮。

##多语言
目前系统支持两种语言，中文和英文。

系统的第一版本为英文版，然后在此基础上产生了第二版，所以第二版可能会出现部分汉化不完全的问题。

#实现
在前端，使用的是```bootstrap 3.0+jquery```实现。后端使用```django 1.4+mysql 5```。

运行在SAE上。目前来说是最省的方案。所以系统可能出现一定程度的不稳定，见谅。

**不支持IE9以下的浏览器。可能会出现部分显示问题。**

由于不是美工出身，所以部分素材来自网络，若有问题，告即删。

#联系我们
如果您发现了任何问题，请让我们知道。Thanks in advance.

hewwcn: hewwcn(at)qq.com

rhain: rhainliu(at)gmail.com

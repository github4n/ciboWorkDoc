在折腾完gitbook的自动部署之后，喊上小伙伴装上Gitbook Editor ，PS：后面都简称‘GE‘，准备大伙一起来开心的写工作文档，可是突然间，duang的一声，两台win7系统的GE都跟我说：‘failed to get server certicertificat’，这特么真的是日了 dog，把我的兴奋劲按在地上摩擦摩擦了。

但抱怨归抱怨，我们还是得去解决问题的是不？

#### 方案一：重装大法 + 配置大法！！！

在经历了无数次的重装，授权，项目重load之后，发现全特么不行，还是跟我说那句英文，好吧，找度娘问问，那句鬼语到底啥意思？  好了，度娘很豪爽的跟我说，对不起，你没有获取到服务器的验证，我就想，难道是github的问题，可是，另一台win10又能完美执行，那就应该还是win7的问题吧。

至此，方案一宣告失败！！

#### 方案二：命令行

既然GE不行，那直接用git更新，推送，行不行能，再把小伙伴的帐号拉进开发组之后，发现，完全没问题啊，简直perfect。那肯定就是这该死的GE的问题，我们总不能在GE上编辑完，然后在傻逼逼的打开个命令行，写两个命令去更新吧。这做法真的low到爆！！

于是，方案二也无疾而终了！

#### 方案三：寻求外国友人的帮助

在经历了刀山火海之后，我发现我是解决不了了，于是我就跑到了gitbook官网的留言版，和github上提issue。（PS：用我那蹩脚的狗级英语，没想到大神还真看懂了！！！） 没想到早上11点提的，下午休斯顿的大神就回了我并发了条链接，按着链接里的方法，给win7装了两补丁之后就特么解决了。。。整个过程加上重启不用5分钟~~~~大神，请在遥远的休斯顿接受我的膜拜，这赛季，火箭必胜！！！

下面，贴上链接地址：[解决问题的链接](https://stackoverflow.com/questions/48985995/gitkraken-and-github-failed-to-get-server-certificate-the-handle-is-in-the-wr)  
![](/assets/1import.png)

这个帖子说引起问题的原因是因为win7的TLS协议，打上两个补丁，然后重启一下电脑，就可以解决了！！！！！

下面是两个补丁的链接：

1、[http://www.catalog.update.microsoft.com/search.aspx?q=kb3140245](http://www.catalog.update.microsoft.com/search.aspx?q=kb3140245)

2、[http://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi](http://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi)

最后，方案三成功胜利，谢谢外国友人！！！


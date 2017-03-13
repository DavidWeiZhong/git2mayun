# git2mayun
这是一个git中码云的使用，其实也是和github中git的使用是一样的，就是学习了一张新的方法而已
想学通过git上传到github的请移步http://blog.csdn.net/two_water/article/details/53512195

先介绍一下git的使用吧，其实呢git的作用就是一个工具而已，和svn是一样的道理的，他只是一个仓库管理员而已，你可以同过git把你的代码上传到本地仓库（就是本地磁盘）,也可以上传到远程服务器（如果你家
公司有联想2010server等的服务器的话，我们通常讲的远程服务器讲的就是像github，和码云那样的公共平台上面的服务器），所以这里也就介绍一下git上传到码云吧，之前的文章也是介绍了git上传到github，但是没有j
介绍git的使用

#git的使用
我也不废话多说了，直接看看官网吧，他们的技术文档非常详细和简单，据说是连猴子都能看懂的技术开发文档
http://backlogtool.com/git-guide/cn/intro/intro1_1.html

#1，把自己的项目上传到码云中
也就是说整个项目是你完成的，你要把你得项目通过git上传到码云中共其他人下载
你也可以移步这里http://www.sxt.cn/info-6043-u-7372.html
好饿，下午再来写一下把。。。。

午休了一下，这两个技术文章绝对能处理你所有的问题
http://blog.csdn.net/lei_notes/article/details/53287447
http://blog.csdn.net/a10615/article/details/52135617

好了，前辈已经帮我们铺好路了，我们要加油
其实遇到的问题就是，应为你上传到码云的时候，由于，你在码云新建的项目有一个readme.md.而你的Android studio 里面没有，所以，你要先pull下载下来，但是你先下载下来的时候，git又会
告诉你有不同的分支，所以git还要设置一下git pull origin master –-allow-unrelated-histories ，这样才不多就解决了问题了

#2，从码云中下载别人的项目
1,android studio 中配置git··
![image](https://github.com/DavidWeiZhong/git2mayun/blob/master/image/3.png)

2，在Android studio中操作，当然你的Android studio 一定要先配置git..
![image](https://github.com/DavidWeiZhong/git2mayun/blob/master/image/1.png)
![image](https://github.com/DavidWeiZhong/git2mayun/blob/master/image/2.png)


基本上你就可以了，然后你改你的项目的时候就可以vcs上传下载啦
![image](https://github.com/DavidWeiZhong/git2mayun/blob/master/image/4.png)

#3 git分支的使用
一般第一次提交都是默认master的，以后要是有了1.0  2.0  3.0 的版本还是要分支的，在码云端要先自己创建一个分支，然后本地pull到本地，然后本地改动了以后再push上云端一开始会叫你选择是上传到那个分支，选择好了后，上传既可以了
#总结

1通过今天的学习，还是从新认识了一下git这个工具，总之就是一个管理员吧，可以把你的项目上传到公共的地方，当时在你上传之前，你先要下载下来你公共服务端没有的代码，和一些分支（第一次上传当然没有问题啦），以后就在这里总结git的各种坑吧
有的时候你拉取分支的时候会不成功，原因可能是你的项目的省略文件与拉去的分支不匹配造成的，所以省略文件尽量要一致

2，git上传到远程，一点要先本地commit，这样你上传到远程万一像复原也是可以的，一般情况下，你直接上传到远程是不可以的，你需要先commit到本地，然后在上传到远程，可是一般情况下，你也不能上传到远程，因为如果有人先与你上传到远程，那么你就要先pull下来了，pull你一般也不能成功，你还要处理一下合并一下代码（这里一般要找当事人进行协调），这样就好了，另外，还原也是分两种的，一种是，你自己改动了代码以后commit到本地，然后又改了一点，然后你想还原，则还原的是你自己改动了的，第二种还原是版本级别的还原了，就是你pull下来别人的代码，然后整个进行还原（版本的还原）

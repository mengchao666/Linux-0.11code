![](https://img.shields.io/github/stars/mengchaobbbigrui/Linux-0.11code)      ![](https://img.shields.io/github/forks/mengchaobbbigrui/Linux-0.11code)      ![](https://img.shields.io/github/issues/mengchaobbbigrui/Linux-0.11code)
## Linux0.11
**“RTFSC – Read The Fucking Source Code :)!”               –Linus Benedict Torvalds**

Linux系统目前发展的如火如荼不管是在嵌入式领域，还是服务器，甚至个人PC都有广泛使用，由此引无数英雄好汉相继加入学习Linux的行列，而这其中定有人想一探Linux内核的究竟。

但是现在Linux内核版本已经5.3.5的版本了，内核相当庞大，几百万行的代码，并不能轻松的阅读。而早期的Linux内核源码比如0.11版本的，代码数量较少不到两万行，而且几乎就是现在内核的精简版本，基本功能原理与内容也都包含，因此非常适合学习。（0.11之前的源码都已丢失，现存的0.10是Ted Ts'o保存下来的，0.11更完善一些）

而且源码面前，了无秘密。相信在读懂源码之后可以对自己的知识能力和解决问题的能力可以更上一层楼，更了解操作系统的原理与设计，深入理解底层的机制，这绝对是内功。


## 教程
阅读Linux内核0.11的教程肯定要有赵炯博士写的书啦。《Linux内核完全注释》。

基于0.11内核《Linux内核完全注释：基于0.11内核(修正版V3.0)》下载链接https://pan.baidu.com/s/19HHrlhcZXyE2GybhRlEHkA

基于0.12内核 2019年最新修正版本《Linux内核完全注释：基于0.12内核(V5.0)》下载链接https://pan.baidu.com/s/1wdoPCeL1cW1nWisw9yrGZg

还有新设计团队写的《图解Linux内核设计的艺术》
下载链接：https://pan.baidu.com/s/1E0E7wv2MUkhjpbja2nhtzw

## 更多内核版本

下载最新的内核请到这里下载[https://www.kernel.org/](https://www.kernel.org/)

下载1.0之前内核可以到这赵炯博士维护的网站下载[http://www.oldlinux.org/Linux.old/](http://www.oldlinux.org/Linux.old/)

## 工具
工欲善其事必先利其器，一个良好的工具，肯定能提高生产力，提高效率。

分析Linux内核这种大型项目在Windows下用sourceinsight是很方便的。具体优点可以自行查询，如果你用过，你肯定会赞同这句话的。如果没用过，可以使用一下，分析这种大型项目这个工具肯定会让你爱不释手的。
![](https://i.loli.net/2019/10/10/YXQ5gsItZhEqa9d.png)
Linux中和sourceinsight差不多的软件名是kscope。

这里我分享source insight3.5版本的，内附激活码和汉化说明，需要的自行下载，https://pan.baidu.com/s/1IKf4ebN08i9LyohXNBhKxQ

3.5版本已经很稳定了，想要用4.0版本的请自行寻找。

使用方法：

(1)要使用SI看代码，首先要创建一个工程。菜单栏：Project->new project。在弹出的对话框中上面输入工程名字（自己起名字，随便写，但是一般要和工程相对应免得时间长了忘记了），下面输入工程文件存放的位置。

(2)工程项目文件和工程中管理的源代码文件目录可以不同，但是我一般习惯放在一起。点确定，进入new project setting，直接点ok进入下一步。

(3)到了向项目中添加文件的步骤。在左侧选择目录，然后点右侧边栏的add tree即可添加，发现添加了xxx个文件进去。

(4)本来应该已经结束了，但是有遗留问题。因为SI软件有个特点，它只能发现自己识别了的文件类型，对于它未识别的文件类型它就看不到。譬如head.S文件就未包含在内，因为SI默认不认识.S后缀的文件。解决方案：自己配置，把.S添加到目录即可。（或者直接把旁边的添加所有文件勾选上）

(5)解决了4中的问题然后再次添加文件。菜单栏　Project->Add and Remove Project Files 再次浏览目录下，再次add tree，发现添加了额外的文件。


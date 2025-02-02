---
date: 2022-08-29
---

# 第一章 贝尔实验室

贝尔实验室做出了大量改变世界的科技成果。最早的是晶体管，由约翰·巴丁（John Bardeen）、沃尔特·布拉顿（Walter Brattain）和威廉·肖克利（William Shockley）于 1947 年在尝试为远距电话线路改进放大器时发明。20 世纪 40 年代，业界亟待出现比真空管在物理上更可靠、耗能更少的设备，这是制造通信装备和构建最早的计算机的必要条件。这种需求推动了对半导体材料的基础研究，晶体管应运而生。

有时地理位置决定一切。

1967 年实习时，我的办公室位于 2 号楼 5 层 8 号梯旁。上班第一天，我坐在办公室里（那些连实习生都有自己办公室的好日子啊），琢磨着该做些什么。上午 11 点，有个年纪略长的家伙出现在门口，说：“嗨，我是 Dick。走，吃午饭去。”

我没听清楚他姓什么。不过我想，行，为什么不呢？那顿午饭怎么吃的我完全不记得了，只记得饭后那位迪克某某就去了其他地方。我沿着走廊找到他办公室门上的名牌，上面写着“Richard Hamming”！这位和善的邻居原来是一位名人。他是纠错码的发明者，也是我选修过的一门数值分析课所用教材的作者。

我和迪克成了好朋友。他观点鲜明，不惧表达，我觉得这会让一些人不爽，但我乐意与他为伍，而且多年以来他的建议令我获益良多。

这是一个合适的博士论文选题，但我进展甚缓。1968 年夏天，当我回到贝尔实验室开始第二段实习期时，我向林申（Shen Lin）请教。那时他刚为经典的“旅行商问题”找到当时最有效的算法：对于一组城市，给出最短路线，必须访问每座城市且每座城市仅访问一次，然后返回。

林申提出了一种图划分算法，这种算法虽然无法保证能得出最优解，但看来可靠。我想出了高效地实现它的路子。我用大量图来做实验，评估该算法在实践中的有用程度。该算法看起来相当有效，但我们没办法找到最优解。我也找了一些有趣的特殊图，对于这些图，可以给出既快又能得到最优解的算法。以上工作的成果对于一篇论文是足够了，在暑期结束时，我已经全获所需。我在秋天着手撰写论文，并于 1969 年 1 月通过毕业答辩（从普林斯顿大学 3 年毕业的乐观估计最后变成了 4 年半毕业）。

1969 年，我正式加入贝尔实验室时，没人告知我具体要做什么事。惯例如此：把你介绍给其他人，让你随意晃荡，去寻找自己的研究课题和协作者。回想起来，这似乎是下马威，但我不记得有什么麻烦。周边有那么多新鲜事在发生，想找点儿东西来研究，或者找个人来合作，根本不成问题。两个夏天之后，我已经认识所有人，也了解了一些项目情况。

直至 1981 年不情不愿地成为部门主管之前，我都是一名普通 MTS。多数管理人员都是“赶鸭子上架”，因为这虽然没有终结个人研究生涯，但必然会拖慢进度，而且照料麾下部门颇具挑战性。但人家自有一套话术来说服你：“反正躲不过，长痛不如短痛吧。”或者有时反过来说：“机不可失。”要么是：“你不上，就会有不怎样的人上了哦！”

# 第 2 章 Unix 雏形（1969）

PDP-7 于 1964 年推出，但计算机领域演进太快，到了 1969 年，它已经过时。这台机器本身不算很强大，只有 8K（8192）个 18 位字长的内存（16 KB），但其图形显示非常漂亮，所以肯就为它写了个太空旅行游戏。在这个游戏里，玩家可以漫游太阳系、探访各个行星。这个游戏有点让人上瘾，我玩了好几个小时。

“在某一时刻，我发现离实现一个操作系统仅有 3 周之遥了。”他需要写三个程序，每周写一个：用来创建代码的编辑器；将代码转换为 PDP-7 能运行的机器语言的汇编器；再加上“内核的外层——操作系统齐活了”。

正在那时，肯的太太休了 3 周假，带着一岁大的儿子去加利福尼亚探望公婆，这样肯就有了 3 周不受打扰的工作时间。正如他在 2019 年一次采访中所说，“一周，一周，再一周，我们就有了 Unix。”无论以何种方式来度量，这都体现了真正的软件生产力。

早期系统有一小群用户，其中当然包括肯和丹尼斯，还有道格·麦基尔罗伊、鲍勃·莫里斯、乔·奥桑纳，以及撞了大运一般的我。每位用户都有一个数字身份编号。有些编号代表系统功能而非人类用户，例如根（root）用户，或者说超级用户，身份编号为 0，此外还有一些特殊编号。人类用户的编号从 4 开始。我记得丹尼斯是 5，肯是 6，我是 9。在初版 Unix 系统中拥有个位数用户身份编号，大概也算略具声望了。

“我只想待在学校，因为……一切尽在掌握。我手艺纯熟。午夜时分，学校的‘怪兽主机’会关闭。我用自己的钥匙打开机房，启动机器，在次日早上 8 点之前，它就一直是我的个人计算机。”

“我很快乐，毫无雄心壮志，是一个没有目标的工作狂。”

大学最后一年，肯选了埃尔温 · 伯利坎普（Elwyn Berlekamp）的课。伯利坎普当时在伯克利分校任教授，后来不久就去了贝尔实验室。毕业后那个夏天，肯没申请读研，因为他觉得自己还不够优秀。

“到那个夏末，（伯利坎普）说：‘你去读这个研究生班吧。’原来他替我申请了读研，而且申请通过了！”

1966 年，肯拿到伯克利分校的硕士学位。贝尔实验室和另外几家公司都想招他，但他明确表态不想去任何一家公司上班。

招聘官一试再试。如肯所言：“贝尔实验室问了 6~8 次，我都拒绝了——也是因为我没有雄心壮志。贝尔实验室招聘官敲我家门，我请他进屋。据他说，我还用姜饼和啤酒招待了他。”（这大概是加利福尼亚的什么古怪减肥饮食吧。）

最后，肯接受邀请，由贝尔实验室支付旅费，去新泽西看看，但是他只答应去一天，而且主要是为了探访高中时代就结识的朋友。他到达贝尔实验室时，被一些名字打动了：

“一到那儿，我就沿计算科学研究中心的走廊漫步，两边办公室门上写的名字如雷贯耳。太震撼了。面试官是两位妙人……其中一位是林申。

“次日，我租车出行。他们不知怎么查到了我的行踪，还在东海岸我停留的第三站留下一份入职邀请书。我拿了那份邀请书，继续下一站两个小时的行程，边开车边考虑。一到达朋友家，我就打电话去实验室，说我接受邀请。”

# 第 3 章 初版（1971）

1127 中心以外的 Unix 早期拥趸中，有一位非常杰出的理论物理学家。为逝者讳，姑且叫他“M- L-”好了。M- L-渴望使用 Unix，他预见到物理学研究将大量使用计算机。他善良而大方，就是话多，能听得你耳朵起茧子。只要他一开口，就谁也就没有办法拦得住他之后一小时的独白。于是，有人在 Unix 房间的门上挖了一个小孔，这样我们就可以在进门前窥视一下，看看他是否在里面。这就是所谓的“L 洞”。

![Unix 房间的浓缩咖啡机和磨豆机](http://yano.oss-cn-beijing.aliyuncs.com/blog/2022-08-29-13-12-42.png)

# 第 4 章 第 6 版（1975）

今天的读者可能很难体会到这一切是做了多大简化之后的结果。早期操作系统中，真实设备的所有复杂情况都会反馈给用户。用户必须知道磁盘名称，了解磁盘的物理结构，如有多少柱面和磁道，以及数据是如何安放在上面。史蒂夫·约翰逊下面这段话让我记起，那时霍尼韦尔主计算机上的分时子系统是多么的笨拙：

“要在霍尼韦尔 TSS 系统上创建文件，必须先进入一个子系统。你得回答 8 个问题：文件的初始尺寸、最大尺寸、名称、设备、谁能读它、谁能写它等。问题逐个提出，你逐个回答。答完所有问题后，操作系统得到这些信息。如果输入错误，文件创建就会失败。这意味着你得再次进入子系统，再次回答所有的问题。难怪文件终于创建时，系统会反馈说‘SUCCESSFUL!’”

管道也许是 Unix 中最引人注目的创新。管道是一种机制，由操作系统提供，并通过 shell 轻松访问。它将程序的输出与另一程序的输入连接起来。操作系统让它发挥作用，只需要一个既简单又自然的 shell 符号就能用起来，结果是得到一种设计和使用程序的新思路。

道格原本想让程序与程序能够随意连接，但如何自然地描述一个无约束图并不那么容易，而且还存在语义上的问题：在程序之间流动的数据必须正确排队，而程序的无管理连接有可能容纳不了那么长的队列。而且肯无论如何也想不出实际应用场景。

但道格继续唠叨，肯继续思考。正如肯所说：“有一天，我想到了：管道。本质上就是管道。”他只花了一小时就在操作系统中添加了管道系统调用。他形容管道是“超级小菜”，因为 I/O 重定向的机制早已存在了。

肯将管道机制添加到 shell，尝试使用。他说，结果“很震撼”。

管道符号是两个命令之间的一道竖杠，简单而优雅。例如，要计算某个目录中的文件数量，可以将 ls 的输出（每个文件一行）用管道导向 wc（计算行数）的输入。

# 第 5 章 第 7 版（1976-1979）

这群来自工业界的相对少量的研究人员何以能写出这么多有影响力的书？

以我之见，有那么几个原因。首先，人们认真对待写作，殚精竭虑。对于其他人的作品来说，他们也是了不起的审读者。道格·麦基尔罗伊是这群人中的魁首。无论什么主题，道格都能发现别人发现不了的错误（有细微错误也有关键错误），别人都没有他那种如炬的眼光。我在贝尔实验室时，无论写了什么都会请道格点评，而他总是如我所请。当他撕裂我的文字时，我感到很惭愧，但这使我成为更好的写作者，同样的事情也发生在其他人身上。

当然，道格并不是唯一的审读者。每个人都慷慨奉献出自己的时间，对同事写的东西不吝给出意见，这不过是文化使然。在其他地方这种情况并不常见，所以贝尔实验室才能那么伟大。

其次，管理层支持图书写作。出版物，包括图书在内，对于维护贝尔实验室在科学界和学术界的声誉非常重要。在管理层的支持下，员工可以全身心地投入到图书写作中。这种全力以赴 6 个月足以基本完成的工作，如果只是业余或在晚上来做，可能需要数年时间。虽然贝尔实验室保留了书籍的版权，但作者可以获得版税，这就更有推动力了。我想我们中没有人是为了赚钱而写书的——实验室没人会蠢到以为写技术书有利可图，但如果图书取得了些许成功，作者就能拿到这笔钱。

# 第 9 章 遗产

不过，我还是很乐观，理由是伟大的创意总来自个体。

例如，早期为 Unix 做出贡献的人很少，可以说核心就是肯·汤普森一人而已。他无疑是我见过的最棒的程序员，也是无人可以比肩的原创思考者。丹尼斯·里奇与肯共同创造了 Unix，他是重要的贡献者。丹尼斯的 C 语言是早期 Unix 发展的核心，至今仍是计算机的通用语言。考察一下程序员们每天使用的语言，这些语言最初往往出自一两个人之手，这很有启发意义。几乎所有主要的编程语言都是如此，包括 Java（詹姆斯·高斯林，James Gosling）、C++（本贾尼·斯特劳斯特鲁普）、Perl（拉里·沃尔，Larry Wall）、Python（吉多·范·罗苏姆，Guido van Rossum）和 JavaScript（布伦丹·艾奇，Brendan Eich）。似乎可以预见，将会继续有新的语言出现，让编程变得更简单、更安全。同样可以预测，不会只有一种语言，然而每种语言都有得有失，无法满足所有目的。

谷歌、Facebook、亚马逊、Twitter、优步（Uber）以及其他从初创企业发展到数十亿美元规模企业的公司，都源于一两个人的聪明想法。这种情况会更多，不过也有可能新想法和新公司一出现，很快就被大公司夺走。聪明的想法可能会被保留下来，发明者也会得到丰厚回报，但大鱼很可能很快就会吃掉小鱼。

# 肯·汤普森

![肯·汤普森 约 1981 年](http://yano.oss-cn-beijing.aliyuncs.com/blog/2022-08-29-13-13-14.png)

“贝尔实验室问了 6~8 次，我都拒绝了——也是因为我没有雄心壮志。”

写了 Unix，2006 年加入谷歌，发明了 Go 语言。

# 丹尼斯·里奇

![丹尼斯·里奇 约 1981 年](http://yano.oss-cn-beijing.aliyuncs.com/blog/2022-08-29-13-13-48.png)

 Unix 和 C 语言，ACM 图领奖（1983 年）

---

coding 笔记、读书笔记、点滴记录，以后的文章也会同步到公众号（Coding Insight）中，大家关注^_^

我的博客地址：[博客主页](https://yano-nankai.notion.site/yano-nankai/Yano-Space-ff42bde7acd1467eb3ae63dc0d4a9f8c)。

![](http://yano.oss-cn-beijing.aliyuncs.com/2019-07-29-qrcode_for_gh_a26ce4572791_258.jpg)
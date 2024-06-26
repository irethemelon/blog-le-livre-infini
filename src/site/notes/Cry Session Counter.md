---
{"dg-publish":true,"permalink":"/cry-session-counter/"}
---


周末，断断续续沉寂了18个小时，给自己写出来了这么个计数程序。今年哭的次数太多了，想找一个看上去很理性的壳子来兜住我这些无处释放的情绪，这样是不是就不用哭那么伤心了？它的名字叫Cry Session Counter，听上去酷酷的不是吗？一个由纯粹的理性搭建起来的不起眼的功能，冷冷的不再有开放性伤口的code和message，却能悄悄装下我大半个情绪世界，好像一个文科生在世界的角落给自己挖的老鼠洞。拍脑门一想，嘿，这不是我大四下学python的时候某个月把我写哭的小作业吗？让我们看看exposure therapy究竟管不管用吧！

后来就自残一样把自己锁书房里钻研代码。在GPT-3.5的倾心帮助下，基础功能很快就能像破车一样运行。我和它说，我的哭泣是分了intensity的，我像教培一样跟查老师解释，哭也有不同的哭啊，我们在代码里补上了这一行，加到了新建按钮的循环里： `intensity_levels = ["bawl", "wail", "weep", "sob", "whimper", "tear up", "wet eyes"]`

我一条一条地过代码检查，才发现查老师认真地乱写了不少内容，突如其来的焦虑让我习惯性地把嘴唇咬出血。随后立刻要去和曲奇见面，于是这个柴火都还没捡齐整的项目就先搁置了。回家的地铁上我装模做样地在手机上研究代码，像是有个什么大开发项目要推进一样，可我一下子难过得直接开始weep。我一边哭又一边蠢笑起来，我心想我都已经开始weep了，计数器这个地方都应该+1了，我程序呢？

它好笑在，我才走到如此基础的第一步，心情就已经跌落谷底。回到书房后我得心应手地盘算起来人生中太多太多让我措手不及的挫败，痛哭流涕着先去洋洋洒洒写完一篇经典的自揭伤疤的文学（[曲奇](https://www.notion.so/a031686fc5704f6fa95dc103aa043b7a?pvs=21) ），爱而不得，爱而不得，写完之后读了好多遍，自恋了一小会儿，心情好了不少。wail计数又得+1了，可程序还是没跑起来。我还想着这程序要怎么优化来着，比如我原本是在weep，后来weep升级成了wail，这规则要怎么写？这视觉要怎么做？我哭得更崩溃了，因为这个我真的写不出来，结局是我哭到三点累睡着了。

第二天起床，继续咬着昨天被咬破的嘴唇，又设计了好几个小时界面。GUI design原来这么复杂的（以下是ADHD典型症状）。

为了居中一堆哭泣intensity的按钮，还要新建一个frame，才能把这一堆按钮打包居中，pack(side=tk.)只能选TOP, BOTTOM, LEFT和RIGHT，pack(anchor=tk.)才能写CENTER，padx和pady也要规定，按钮的位置才能好看（你姐的正职工作调研没白做）。

为了修改字体，又去查了Windows能显示的字体，不过字体好多哦，我看到C开头的那一堆字体就没办法往后看了，选了Candara（并查到candara是意大利语里面的一种锅…），肯定错过了不少别的漂亮字体吧。最后学明白了加粗、下划线怎么写。

为了改背景、字体和按钮的颜色，又查了CSS colors，发现有好多名字取得好漂亮的颜色，mistyrose，lavenderblush，slategrey，whitesmoke，goldenrod，magneta，ghostwhite，royalblue，peachpuff，honeydew，darkseagreen，blanchediamond，lemonchiffon，cornflowerblue，papayawhip，被这些和世界紧紧相连的颜色和命名美得耽搁了半个小时。

终于走到测试的一步，发现计数逻辑一塌糊涂，于是又装模做样地拿出草稿本开始算逻辑，在python help里学这样那样的函数，在代码里填这样那样的参数，眼含热泪去对抗我从小没学明白的数学和逻辑，总算把程序调明白了。现在我终于可以在弹窗里输入我哭泣的理由，输入后才能计数，不输入不算数！wet eyes+1。

程序run起来之后，我的心前所未有地空了。

写这个程序，其实只有10%的目的是为了记录我接下来这年的情绪，剩余的90%都是赌气。是中学数学考试做到每个大题的倒数第一二题都会哭，最后直接不做，所以分数永远都徘徊在120，以至于26岁了还会在焦虑的梦里relive那些瞬间，哭着醒来，然后无助地爱上一堆无情的理工男。是所有语文老师都说我没有感情、适合做理科生这样的声音。是小羊每天反反复复念叨让我学程序，是曲奇吃饭时跟我说你写吧真的很简单小羊的中台又不会被我们干垮。是我内在的割裂，我坚硬的外壳，我脆弱的内心。是他，是我，是想证明我一个人也可以，我不需要去追求他。是想证明我不需要高大的、可爱的、自由的、沉稳的、独立的、坚定的、有趣的、错误的他来成为我的savior，soulmate，wings。是想尝试放弃走进他的世界，放弃那个卑怯的、总是需要被一段“-ship”托举起来的自己。

如果是我，我一个人，会怎么做？

就像周末这两天一样做，哭着做，和乱教的查老师一起做，哭着做，power through，咬破嘴唇power through，然后收获一颗今天这样的，轻飘飘的、空荡荡的心。

如果是前夫，他和我，会怎么做？

我会像个什么都没想好的产品经理一样去给前夫提需，前夫会因为这个程序太没用，跟我说有空给你写一个，这个简单，然后再也不做。最后被我问起，他会说，“你这个是重复造轮子”，“GitHub上的人都不稀罕写你这个”。我还是会像现在这样赌着一肚子的气去“证明”，去哭着问查老师，然后copy一段我一开始啥也看不懂的代码到pycharm里哭着研读。等我的代码稍有成色，他就会走到我的屏幕前问我，你搞懂了吗？你能行吗？你给我解释一下这个函数什么意思呢？等我真正遇到了我无法解决的问题、向他求助，他就会装模做样地让我离开我的位置，坐下来从头开始学习那些他也没用过的库，跟我说这个简单，然后无情地用他的ego来耽搁我的工作进度。可是那些库我都已经研究明白了，我只需要找一下语法怎么写就能用了。

如果是他，他和我，会怎么做？

一切到这里都只存在在不会落地的幻梦中。我这颗轻飘飘的、空荡荡的心啊，缺了那么大那么大一个，高大的、可爱的、自由的、沉稳的、独立的、坚定的、有趣的、错误的他，要他来成为我的savior，soulmate，wings。我原本可以飞的，真的。

我最终证明了什么呢？我其实还是做不出数学考试题，没办法像曲奇一样攻打小羊的中台，没办法不爱无情的理工男，没办法不需要“-ships”，也没办法填满我轻飘飘的、空荡荡的心。

今天看了病回来再看Cry Session Counter的代码觉得里面的命名都好好笑，什么”display_cry_data”之类的，正经的程序里会有cry这样的词吗？是人文社科兜起来了这个程序。因为没有我，就没有这个没人在意的小窗口了呀。
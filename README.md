Github 使用指南
===============



### Github 是什么

- [怎样一个网站][github-baidu]：一个程序托管网站，一个社会化编程平台（Social Coding）
- Github 使用 Git 版本控制，Git 作为一个版本控制工具有什么特点：
    - Git 是目前世界上最先进的分布式版本控制系统（没有之一）。
	- 特点是高端大气上档次！（[廖雪峰语][liaoxuefeng-git]）
- Github 对于程序员的意义：
    - 你要知道 Github 被中国的防火长城封锁过几次，在多人联名抗议下才解锁。李开复也发博声援：
    - ![][github-blocked]
- 竞争对手：
    - 国外的 BitBucket，以及
	- 中国的 Github 克隆版 GitCafe
- 现在请注册一个 Github 账户（必须的），有账户的请登录



### Git 常用流程

- 详细戳 Git 教程：[廖雪峰 Git 教程][git-liaoxuefeng]，或者 [我的 Progit 笔记][pro-git-notes]
- 简单地说 Git 记录了文档的状态和状态间的变动，所有记录项分为三个状态：
    - modified（修改了）
	- staged（提交了）
	- committed（提交确认了）。
- Git 命令分为三个部分：git + 命令 + 参数等，不如：
    - `git clone url` 从 url（需要合法的 git repo 才行） 克隆一个副本到本地当前目录
	- `git commit -m "message"` 把修改提交并记录
- 一个通常的 Git 流程是：
    - `git clone git@github.com:district10/new-repo.git`
	    - 把一个云端 repo 复制下来
		- 复制别人的 repo 用 https 协议，复制自己的 repo 用 git 协议，直接在本地创建一个 git repo 则使用 `git init`
		- 一个 git repo 有一些文档来记录变化，他们是隐藏的。
    - `git add -A`
	    - 在每次修改后，修改的文档的状态就从 clean（committed） 变成 modified
		- 使用这个命令把所有内容提交，状态变成 staged
    - `git commit -m "提交记录"`
	    - 把修改 commit，比如：”修正了一个拼写错误“（Fixed Typo），但这时候只是本地修改好了，云端（Github 端）没有同步。
    - `git push`
	    - 把修改同步到云端，最简单地方式就是 git push
		- 多人合作的时候，每次先把本地修改 commit，再 push 到 云端。再把别人的修改 `git pull` 下来。

		

### 使用 Github：前提

- 联网的电脑
- 网页登入（在网页上也可以很方便的查看别人代码，克隆别人的 repo）
- 控制台 SSH 连接（用 SSH 登入方便地同步代码，版本控制）
- 最好学习一下 Markdown 的使用
    - Github 上的 README 文档很多都是用 Markdown 写成（以 `.md` 结尾的文件）
	- 学习 Markdown 可参考我的博客：[Markdown 简明教程][markdown]

	
	
### Github 教程：Step by Step

- 首先按照教程配置 Git：
    - [Windows 用户][git-windows]
	- Linux 用户那就太简单了，直接敲命令一行搞定。如 Ubuntu 用户使用指令：`apt-get install git`
- [新建一个 Repo][new-repo-guide]




---

## 附录

#### 为什么要学习 Git

- XDite 的博文：[有效提升大學生競爭力 -- 用 Git Pull Request 收作業][git-homework]


#### 文档撰写与 Coding 规范

- [写博客，撰写文档通用规范][convensions-writing]
- [Coding 规范][convensions-coding]


#### 如有疑问

如有疑问请到 Issue 提问：

![][how-to-issues]




[git-homework]: http://blog.xdite.net/posts/2014/06/18/git-pull-request-homework
[convensions-writing]: https://gitcafe.com/Guide-of-Coding/general-convensions
[convensions-coding]: https://gitcafe.com/Guide-of-Coding/coding-conventions
[how-to-issues]: http://whudoc.qiniudn.com/github-guide/img/issues.png

[github-baidu]: http://baike.baidu.com/view/3366456.htm
[git-liaoxuefeng]: http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000
[pro-git-notes]: http://jianshu.io/p/db84ee45f16c
[liaoxuefeng-git]: http://www.liaoxuefeng.com/wiki/0013739516305929606dd18361248578c67b8067c8c017b000/001373962845513aefd77a99f4145f0a2c7a7ca057e7570000
[github-blocked]: http://whudoc.qiniudn.com/github-guide/img/github-blocked.png
[git-windows]: https://github.com/whudoc/github-guide/blob/master/%E9%85%8D%E7%BD%AE-Windows.md
[new-repo-guide]: https://github.com/whudoc/github-guide/blob/master/%E6%96%B0%E5%BB%BARepo.md
[markdown]: http://jianshu.io/p/7bd23251da0a
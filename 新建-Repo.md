# 如何在 GitHub 上新建一个 Repository



### 【1】

首先去 GitHub 主页 https://github.com ，在右上角点击 New Repository

![][new-repo-a]



### 【2】

然后输入新 Repo 的名称，输入 Repo 说明，选择 Public（Private 要收费），
勾选生成 `README` 文档，选择一个 `.gitignore` 文件（也可不选），
选择一个协议，这里我选了 `GPL v3`，整个如下：

![][new-repo-b]

这样，就在 GitHub 上新建了一个 Repo，如下：

![][new-repo-c]





### 【3】

然后把这个 Repo 用 Git 克隆下来，先到如上图右下角，复制 SSH 链接：

`git@github.com:district10/new-repo.git`（复制自己的 Repo 用 SSH，别人的用 HTTPS）

然后到本地目录，比如这个 `github` 文件夹下，右键打开 Git Bash，输入

```bash
git clone git@github.com:district10/new-repo.git
```

如图：

![][new-repo-d]

![][new-repo-e]

克隆好后当前文件夹下就有了 `new-repo` 文件夹，如图：

![][new-repo-f]





### 【4】

进入文件夹，用 Notepad++ 打开 `README.md` 文件：

![][new-repo-g]

简单地修改，添加一行 “【这是新入的一行。来自 Notepad++】”：

![][new-repo-h]

然后在 `new-repo` 文件夹打开 Git Bash 提交修改并 Push 到 GitHub：

![][new-repo-i]

再到自己的 GitHub 上，查看，发现修改已经提交上去了：

![][new-repo-j]




### 【完】

这就是在 GitHub 上新建一个 Repo 的过程。以后修改之后，再

```bash
git add -A # 与 git add README.md 不同的是，这个命令一次添加所有修改了的文档
git commit -m "Msg"
git push
```

即可把代码同步到 GitHub。Git 在编写代码时可以很好的控制版本，深入的学习，可以参考 [最好的 Git 进阶材料][progit-learn-more]






[new-repo-a]: http://whudoc.qiniudn.com/github-guide/img/new-repo-a.png
[new-repo-b]: http://whudoc.qiniudn.com/github-guide/img/new-repo-b.png
[new-repo-c]: http://whudoc.qiniudn.com/github-guide/img/new-repo-c.png
[new-repo-d]: http://whudoc.qiniudn.com/github-guide/img/new-repo-d.png
[new-repo-e]: http://whudoc.qiniudn.com/github-guide/img/new-repo-e.png
[new-repo-f]: http://whudoc.qiniudn.com/github-guide/img/new-repo-f.png
[new-repo-g]: http://whudoc.qiniudn.com/github-guide/img/new-repo-g.png
[new-repo-h]: http://whudoc.qiniudn.com/github-guide/img/new-repo-h.png
[new-repo-i]: http://whudoc.qiniudn.com/github-guide/img/new-repo-i.png
[new-repo-j]: http://whudoc.qiniudn.com/github-guide/img/new-repo-j.png
[progit-learn-more]: http://book.douban.com/review/6465637/
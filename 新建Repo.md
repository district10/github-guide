# 如何在 Github 上新建一个 Repository

首先去 Github 主页 https://github.com ，在右上角点击 New Repository

![][new-repo-a]

然后输入新 Repo 的名称，输入 Repo 说明，选择 Public（Private 要收费），勾选生成 README 文档，选择一个 gitignore 文件（也可不选），选择一个协议，这里我选了 GPL v3，整个如下：

![][new-repo-b]

这样，就在 Github 上新建了一个 Repo，如下：

![][new-repo-c]

然后把这个 Repo 用 Git 克隆下来，先到如上图右下角，复制 SSH 链接：`git@github.com:district10/new-repo.git`（复制自己的 Repo 用 SSH，别人的用 https）

然后到本地目录，比如这个 github 文件夹下，右键打开 Git Bash，输入 `

```bash
git clone git@github.com:district10/new-repo.git
```

如图：

![][new-repo-d]

![][new-repo-e]

克隆好后当前文件夹下就有了 `new-repo` 文件夹，如图：

![][new-repo-f]

进入文件夹，用 Notepad++ 打开 `README.md` 文件：

![][new-repo-g]

简单地修改，添加一行 “【这是新入的一行。来自 Notepad++】”：

![][new-repo-h]

然后在 `new-repo` 文件夹打开 Git Bash 提交修改并 push 到 Github：

![][new-repo-i]

再到自己的 Github 上，查看，发现修改已经提交上去了：

![][new-repo-j]







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
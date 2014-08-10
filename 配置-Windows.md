Windows 系统 Git 配置
=====================




### 下载 Git for Windows

Git 需要安装使用，到 [Git Scm][git-scm] 下载 Windows 版本：Git for Windows。
因下载需要翻墙，这里提供一个备份：[Git-1.8.3][git-archive]。版本有点老，但完全够用了。




### 安装 Git for Windows

【1】 双击如下图标（【右键 - 以管理员身份运行】响应更快），开始安装

![][git-for-windows]

【2】 下一步，同意 GNU General Public License

【3】 选择组件，默认即可

![][git-setup-a]

【4】 选择 Git Bash，Bash 是一种命令行

![][git-setup-b]

【5】 选择 Git 换行符工作方式（Windows，Unix/Linux，Mac OS 的换行符各不相同）

![][git-setup-c]

【6】 安装完成，在资源管理器里右键出现了 Git Bash 和 Git GUI 选项

![][git-bash-gui]





### 使用 Git Bash

【1】 打开 Git Bash

在某一文件夹下右键单击打开 Git Bash，这是一个命令行环境，就像 Windows 下的 CMD，PowerShell 或者 Linux 下的 Bash，Zsh

【2】 Hello Git Bash

试着输入，`echo Hello Git Bash`，回车，就有：

![][git-hello]

顺便把自己的用户名和邮箱配置一下：（把用户名和邮箱改成自己 Github 账号对应的用户名邮箱）
 
```bash
git config --global user.name "district10"
git config --global user.email "gnat_tang@yeah.net"
```

【3】 克隆一个 Github Repository

克隆（Clone）就是把代码复制到本地，到 GitHub 上找个 Repo，比如：https://github.com/alols/xcape

在 Git Bash 里输入 `git clone https://github.com/alols/xcape`，回车，就有：

![][git-clone-https]


【4】 配置 SSH

首先打开 Git Bash（不论在哪个文件夹都行），然后输入 `cd ~/.ssh` 把目录跳转到自己用户的 `.ssh` 目录下；（如果失败，则输入 `cd ~ && mkdir .ssh && cd .ssh`）

输入 `ls` （打印目录）应该输出为空；

输入 `ssh-keygen.exe -t rsa -C "your-email"` （换成你的邮箱），回车，有：

![][gen-ssh-a]

等待你输入目录，直接使用默认的，回车即可；

![][gen-ssh-b]

等待你输入密码，可以不设置（方便自己），回车两次即可；

然后 SSH 密钥公钥就生成好了，用 ls 看一下（输入 `ls`)，查看 生成的 公钥，并拷贝到剪贴板：

![][gen-ssh-c]

到 Github 里设置 SSH，如下：

【Step 1】

![][gen-ssh-d]

【Step 2】

![][gen-ssh-e]

保存好就可以了。






### 编辑器选择

Geek 的编辑器有 Emacs，Vim，但是推荐大家使用 Notepad++，这个编辑器简单好用。而且有便携版，解压即可使用。

这里提供一个 Portable 版本下载：http://download.tuxfamily.org/notepadplus/6.6.8/npp.6.6.8.bin.7z





[git-scm]: http://www.git-scm.com/downloads
[git-archive]: http://whudoc.qiniudn.com/github-guide/Git-1.8.3-preview20130601.exe
[git-for-windows]: http://whudoc.qiniudn.com/github-guide/img/git-for-windows.png

[git-setup-a]: http://whudoc.qiniudn.com/github-guide/img/git-setup-components.png
[git-setup-b]: http://whudoc.qiniudn.com/github-guide/img/git-setup-gitbash.png
[git-setup-c]: http://whudoc.qiniudn.com/github-guide/img/git-setup-lineendings.png

[git-bash-gui]: http://whudoc.qiniudn.com/github-guide/img/gitbash-gitgui.png
[git-hello]: http://whudoc.qiniudn.com/github-guide/img/git-hello.png
[git-clone-https]: http://whudoc.qiniudn.com/github-guide/img/git-clone-https.png

[gen-ssh-a]: http://whudoc.qiniudn.com/img/gen-ssh-a.png
[gen-ssh-b]: http://whudoc.qiniudn.com/img/gen-ssh-b.png
[gen-ssh-c]: http://whudoc.qiniudn.com/img/gen-ssh-c.png
[gen-ssh-d]: http://whudoc.qiniudn.com/img/gen-ssh-d.png
[gen-ssh-e]: http://whudoc.qiniudn.com/img/gen-ssh-e.png
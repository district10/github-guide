Windows 系统 Git 配置
=====================

### 下载 Git for Windows

Git 需要安装使用，到 [Git Scm][git-scm] 下载 Windows 版本：Git for Windows。
因下载需要翻墙，这里提供一个备份：[Git-1.8.3][git-archive]。版本有点老，但完全够用了。




### 安装 Git for Windows

1. 双击如下图标（【右键 - 以管理员身份运行】响应更快），开始安装

![][git-for-windows]

2. 下一步，同意 GNU General Public License

3. 选择组件，默认即可

![][git-setup-a]

4. 选择 Git Bash，Bash 是一种命令行

![][git-setup-b]

5. 选择 Git 换行符工作方式（Windows，Unix/Linux，Mac OS 的换行符各不相同）

![][git-setup-c]

6. 安装完成，在资源管理器里右键出现了 Git Bash 和 Git GUI 选项

![][git-bash-gui]



### 使用 Git Bash

1. 打开 Git Bash

在某一文件夹下右键单击打开 Git Bash，这是一个命令行环境，就像 Windows 下的 CMD，PowerShell 或者 Linux 下的 Bash，Zsh

2. Hello Git Bash

试着输入，`echo Hello Git Bash`，回车，就有：

![][git-hello]

3. 克隆一个 Github Repository

克隆（Clone）就是把代码复制到本地，到 Github 上找个 Repo，比如：https://github.com/alols/xcape

在 Git Bash 里输入 `git clone https://github.com/alols/xcape`，回车，就有：

![][git-clone-https]


4. 配置 SSH







[git-scm]: http://www.git-scm.com/downloads
[git-archive]: http://whudoc.qiniudn.com/github-guide/Git-1.8.3-preview20130601.exe
[git-for-windows]: http://whudoc.qiniudn.com/github-guide/img/git-for-windows.png

[git-setup-a]: http://whudoc.qiniudn.com/github-guide/img/git-setup-components.png
[git-setup-b]: http://whudoc.qiniudn.com/github-guide/img/git-setup-gitbash.png
[git-setup-c]: http://whudoc.qiniudn.com/github-guide/img/git-setup-lineendings.png

[git-bash-gui]: http://whudoc.qiniudn.com/github-guide/img/gitbash-gitgui.png
[git-hello]: http://whudoc.qiniudn.com/github-guide/img/git-hello.png
[git-clone-https]: http://whudoc.qiniudn.com/github-guide/img/git-clone-https.png
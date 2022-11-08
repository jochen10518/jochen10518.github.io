## 安装Git

<!-- tabs:start -->

#### **Mac**

Mac系统通常预安装了 **Git** 命令。打开终端 **Terminal**，输入 `git` 指令，如有以下输出，则系统已安装 **Git**。
           
<img src="_media/repo/gitmac.png" width = "800" alt="homepage" align=center />

若系统未安装 Git，请参照[Git官方地址](https://git-scm.com/download/mac)下载安装。

#### **Windows**

访问[Git官方地址](https://git-scm.com/download/win)，根据自己电脑配置，下载 **Standalone Installer** 下面`64-bit Git for Windows Setup`安装。（一般Windows系统为64位，请查看自己电脑的系统版本是否下载32位）

下载完成后，根据安装程序指引完成安装。使用Git Bash 命令行进行Git操作。（你也可以使用其他的命令行工具，如 Windows Powershell，详情参照[微软官方文档](https://learn.microsoft.com/zh-cn/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.2) ）

<!-- tabs:start -->

#### **Git安装**

<img src="_media/repo/gitinstall.png" width = "800" alt="homepage" align=center />

#### **Git Bash**

<img src="_media/repo/gitbash.png" width = "800" alt="homepage" align=center />

#### **Powershell**

<img src="_media/repo/windowsterminal.png" width = "800" alt="homepage" align=center />

<!-- tabs:end -->

<!-- tabs:end -->

## Git提交代码

使用命令行（*Mac Terminal/iTerm2* 或 *Windows Git Bash/Powershell*） **Git** 克隆/提交代码需要设置权限。你可以在代码仓文件列表的右上方找到 **项目链接**。通常有两种方式克隆代码仓，`https` 和 `ssh`。

<!-- tabs:start -->

#### **HTTPS**

使用 `https` 地址克隆项目，操作 `git pull/push` 到的时候需要输入账号密码。你可以 `cd` 项目根目录，输入 `git config --global credential.helper store` 将你的账户密保保存到本地文本。 首次输入后，便不再需要输入账号密码。

```shell
#克隆代码仓
$ git clone https://git.openi.org.cn/chenzh/chenz202211041026224.git
$ cd quickstart

#提交代码
$ git add .
$ git commit -m 'update'
$ git push
username: chenzh
password: 🔑

#保存账户密码
$ git config --global credential.helper store
```

#### **SSH**

使用 `ssh` 链接克隆代码仓需要 **在本地生成ssh密钥** -> **配置ssh密钥** -> **添加ssh密钥到你的启智账号**。

具体步骤请参考[Github SSH Gnerating](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)。



<!-- tabs:end -->
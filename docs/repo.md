### 代码仓

代码仓是项目的首页，也是项目的核心。

### 安装Git


<!-- tabs:start -->

#### **Mac**

Mac系统通常预安装了 **Git** 命令。打开终端 **Terminal**，输入 `git` 指令，如有以下输出，则系统已安装 **Git**。
```shell                                                                              
> git
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone     Clone a repository into a new directory
   init      Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add       Add file contents to the index
   mv        Move or rename a file, a directory, or a symlink
   restore   Restore working tree files
   rm        Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect    Use binary search to find the commit that introduced a bug
   diff      Show changes between commits, commit and working tree, etc
   grep      Print lines matching a pattern
   log       Show commit logs
   show      Show various types of objects
   status    Show the working tree status

grow, mark and tweak your common history
   branch    List, create, or delete branches
   commit    Record changes to the repository
   merge     Join two or more development histories together
   rebase    Reapply commits on top of another base tip
   reset     Reset current HEAD to the specified state
   switch    Switch branches
   tag       Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.
```

若系统未安装 Git，请参照[Git官方地址](https://git-scm.com/download/mac)下载安装。

#### **Windows**

访问[Git官方地址](https://git-scm.com/download/win)，根据自己电脑配置，下载 **Standalone Installer** 下面`64-bit Git for Windows Setup`安装。（一般Windows系统为64位，请查看自己电脑的系统版本是否下载32位）

下载完成后，根据安装程序指引完成安装。使用Git Bash 命令行进行Git操作。（你也可以使用其他的命令行工具，如 Windows Powershell，详情参照[微软官方文档](https://learn.microsoft.com/zh-cn/powershell/scripting/install/installing-powershell-on-windows?view=powershell-7.2) ）

<!-- tabs:end -->


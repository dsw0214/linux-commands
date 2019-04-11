# linux 命令
## Document Description（文档说明）
> 本文提供了Linux/Unix中最常用命令的实用示例。

## Table of Contents (目录)

###  线上查询及帮助命令
> #####  [man 命令](https://github.com/dsw0214/linux-commands/blob/master/man.md "man 命令") : 查看命令帮助,命令的词典,更复杂的还有info,但不常用
> #####  [help 命令](https://github.com/dsw0214/linux-commands/blob/master/help.md "help 命令") : 查看 Linux I内置命令的帮助,比如cd命令
> #####  [whatis 命令](https://github.com/dsw0214/linux-commands/blob/master/whatis.md "whatis 命令") : 用于查询一个命令执行什么功能，并将查询结果打印到终端上

###  用户管理命令
> #####  [useradd 命令](https://github.com/dsw0214/linux-commands/blob/master/useradd.md "useradd 命令") : 添加用户
> #####  [usermod 命令](https://github.com/dsw0214/linux-commands/blob/master/usermod.md "usermod 命令") : 修改系统已经存在的用户属性
> #####  [userdel 命令](https://github.com/dsw0214/linux-commands/blob/master/userdel.md "userdel 命令") : 删除用户
> #####  [groupadd 命令](https://github.com/dsw0214/linux-commands/blob/master/groupadd.md "groupadd 命令") : 添加用户组
> #####  [passwd 命令](https://github.com/dsw0214/linux-commands/blob/master/passwd.md "passwd 命令") : 修改用户密码
> #####  [chage 命令](https://github.com/dsw0214/linux-commands/blob/master/chage.md "chage 命令") : 修改用户密码有效期限
> #####  [id 命令](https://github.com/dsw0214/linux-commands/blob/master/id.md "id 命令") : 查看用户的uid,gid及归属的用户组
> #####  [su 命令](https://github.com/dsw0214/linux-commands/blob/master/su.md "su 命令") : 切换用户身份
> #####  [visudo 命令](https://github.com/dsw0214/linux-commands/blob/master/visudo.md "visudo 命令") : 编辑/etc/sudoers文件的专属命令
> #####  [sudo 命令](https://github.com/dsw0214/linux-commands/blob/master/su.md "sudo 命令") : 以另外一个用户身份(默认root用户)执行事先在 sudoers文件允许的命令

###  进程管理相关命令
> #####  [bg 命令](https://github.com/dsw0214/linux-commands/blob/master/bg.md "bg 命令") : 将一个在后台暂停的命令,变成继续执行(在后台执行)
> #####  [fg 命令](https://github.com/dsw0214/linux-commands/blob/master/fg.md "fg 命令") : 将后台中的命令调至前台继续运行
> #####  [jobs 命令](https://github.com/dsw0214/linux-commands/blob/master/jobs.md "jobs 命令") : 查看当前有多少在后台运行的命令
> #####  [kill 命令](https://github.com/dsw0214/linux-commands/blob/master/kill.md "kill 命令") : 终止进程
> #####  [killall 命令](https://github.com/dsw0214/linux-commands/blob/master/killall.md "killall 命令") : 通过进程名终止进程
> #####  [pkill 命令](https://github.com/dsw0214/linux-commands/blob/master/pkill.md "pkill 命令") : 通过进程名终止进程
> #####  [crontab 命令](https://github.com/dsw0214/linux-commands/blob/master/crontab.md "crontab 命令") : 定时任务命令
> #####  [ps 命令](https://github.com/dsw0214/linux-commands/blob/master/ps.md "ps 命令") : 显示进程的快照
> #####  [nice 命令](https://github.com/dsw0214/linux-commands/blob/master/nice.md "nice 命令"): 调整程序运行的优先级
> #####  [renice 命令](https://github.com/dsw0214/linux-commands/blob/master/renice.md "renice 命令"): 调整程序运行的优先级
> #####  [nohup 命令](https://github.com/dsw0214/linux-commands/blob/master/nohup.md "nohup 命令") : 忽略挂起信号运行指定的命令
> #####  [pgrep 命令](https://github.com/dsw0214/linux-commands/blob/master/pgrep.md "pgrep 命令") : 查找匹配条件的进程
> #####  [runlevel1 命令](https://github.com/dsw0214/linux-commands/blob/master/runlevel1.md "runlevel1 命令") : 查看系统当前运行级别
> #####  [init 命令](https://github.com/dsw0214/linux-commands/blob/master/init.md "init 命令") : 切换运行级别
> #####  [service 命令](https://github.com/dsw0214/linux-commands/blob/master/service.md "service 命令") : 启动、停止、重新启动和关闭系统服务,还可以显示所有系统服务的当前状态

###  文件和目录操作命令
> #####  [ls 命令](https://github.com/dsw0214/linux-commands/blob/master/ls.md "ls 命令") : 全拼1ist,功能是列出目录的内容及其内容属性信息
> #####  [cd 命令](https://github.com/dsw0214/linux-commands/blob/master/cd.md "cd 命令") : 全拼 change directory,功能是从当前工作目录切换到指定的工作目录
> #####  [cp 命令](https://github.com/dsw0214/linux-commands/blob/master/cp.md "cp 命令") : 全拼copy,其功能为复制文件或目录
> #####  [find 命令](https://github.com/dsw0214/linux-commands/blob/master/find.md "find 命令") : 查找的意思,用于查找目录及目录下的文件
> #####  [mkdir 命令](https://github.com/dsw0214/linux-commands/blob/master/mkdir.md "mkdir 命令") : 全拼 make directories,其功能是创建目录
> #####  [mv 命令](https://github.com/dsw0214/linux-commands/blob/master/mv.md "mv 命令") : 全拼move,其功能是移动或重命名文件
> #####  [pwd 命令](https://github.com/dsw0214/linux-commands/blob/master/pwd.md "pwd 命令") : 全拼 print working directory,其功能是显示当前工作目录的绝对路径
> #####  [rename 命令](https://github.com/dsw0214/linux-commands/blob/master/rename.md "rename 命令") : 用于重命名文件
> #####  [rm 命令](https://github.com/dsw0214/linux-commands/blob/master/rm.md "rm 命令") : 全拼 remove,其功能是删除一个或多个文件或目录
> #####  [rm 命令](https://github.com/dsw0214/linux-commands/blob/master/rm.md "rm 命令")dir : 全拼 remove empty directories,功能是删除空目录
> #####  [touch 命令](https://github.com/dsw0214/linux-commands/blob/master/touch.md "touch 命令") : 创建新的空文件,改变已有文件的时间戳属性
> #####  [tree 命令](https://github.com/dsw0214/linux-commands/blob/master/tree.md "tree 命令") : 功能是以树形结构显示目录下的内容
> #####  [basename 命令](https://github.com/dsw0214/linux-commands/blob/master/basename.md "basename 命令") : 显示文件名或目录名
> #####  [dirname 命令](https://github.com/dsw0214/linux-commands/blob/master/dirname.md "dirname 命令") : 显示文件或目录路径
> #####  [chattr 命令](https://github.com/dsw0214/linux-commands/blob/master/chattr.md "chattr 命令") : 改变文件的扩展属性
> #####  [file 命令](https://github.com/dsw0214/linux-commands/blob/master/file.md "file 命令") : 显示文件的类型
> #####  [md5 命令](https://github.com/dsw0214/linux-commands/blob/master/md5.md "md5 命令") : 计算和校验文件的MD5值
> #####  [md5sum 命令](https://github.com/dsw0214/linux-commands/blob/master/md5sum.md "md5sum 命令") : 计算和校验文件的MD5值

###  信息显示命令
> #####  [uname 命令](https://github.com/dsw0214/linux-commands/blob/master/uname.md "uname 命令") : 显示操作系统相关信息的命令
> #####  [hostname 命令](https://github.com/dsw0214/linux-commands/blob/master/hostname.md "hostname 命令") : 显示或者设置当前系统的主机名
> #####  [dmesg 命令](https://github.com/dsw0214/linux-commands/blob/master/dmesg.md "dmesg 命令") : 显示开机信息,用于诊断系统故障
> #####  [uptime 命令](https://github.com/dsw0214/linux-commands/blob/master/uptime.md "uptime 命令") : 显示系统运行时间及负载
> #####  [stat 命令](https://github.com/dsw0214/linux-commands/blob/master/stat.md "stat 命令") : 显示文件或文件系统的状态
> #####  [du 命令](https://github.com/dsw0214/linux-commands/blob/master/du.md "du 命令") : 计算磁盘空间使用情况
> #####  [df 命令](https://github.com/dsw0214/linux-commands/blob/master/df.md "df 命令") : 报告文件系统磁盘空间的使用情况
> #####  [top 命令](https://github.com/dsw0214/linux-commands/blob/master/top.md "top 命令") : 实时显示系统资源使用情况
> #####  [free 命令](https://github.com/dsw0214/linux-commands/blob/master/free.md "free 命令") : 查看系统内存
> #####  [date 命令](https://github.com/dsw0214/linux-commands/blob/master/date.md "date 命令") : 显示与设置系统时间
> #####  [cal 命令](https://github.com/dsw0214/linux-commands/blob/master/cal.md "cal 命令") : 查看日历等时间信息

###  系统权限及用户授权相关命令
> #####  [chmod 命令](https://github.com/dsw0214/linux-commands/blob/master/chmod.md "chmod 命令") : 改变文件或目录权限
> #####  [chown 命令](https://github.com/dsw0214/linux-commands/blob/master/chown.md "chown 命令") : 改变文件或目录的属主和属组
> #####  [chgrp 命令](https://github.com/dsw0214/linux-commands/blob/master/chgrp.md "chgrp 命令") : 更改文件用户组
> #####  [umask 命令](https://github.com/dsw0214/linux-commands/blob/master/umask.md "umask 命令") : 显示或设置权限掩码

###  系统管理与性能监视命令
> #####  [chkconfig 命令](https://github.com/dsw0214/linux-commands/blob/master/chkconfig.md "chkconfig 命令") : 管理 ELinux系统开机启动项
> #####  [vmstat 命令](https://github.com/dsw0214/linux-commands/blob/master/vmstat.md "vmstat 命令") : 虚拟内存统计
> #####  [mpstat 命令](https://github.com/dsw0214/linux-commands/blob/master/mpstat.md "mpstat 命令") : 显示各个可用CPU的状态统计
> #####  [iostat 命令](https://github.com/dsw0214/linux-commands/blob/master/iostat.md "iostat 命令") : 统计系统I0
> #####  [sar 命令](https://github.com/dsw0214/linux-commands/blob/master/sar.md "sar 命令") : 全面地获取系统的CPU、运行队列、磁盘I/0、分页(交换区)、内存、CPU中断和网络等性能数据
> #####  [ipcs 命令](https://github.com/dsw0214/linux-commands/blob/master/ipcs.md "ipcs 命令") : 用于报告Linux中进程间通信设施的状态,显示的信息包括消息列表、共享内存和信号量的信息
> #####  [lpcrm 命令](https://github.com/dsw0214/linux-commands/blob/master/lpcrm.md "lpcrm 命令") : 用来删除一个或更多的消息队列、信号量集或者共享内存标识
> #####  [strace 命令](https://github.com/dsw0214/linux-commands/blob/master/strace.md "strace 命令") : 用于诊断、调试 Linux用户空间跟踪器我们用它来监控用户空间进程和内核的交互,比如系统调用、信号传递、进程状态变更等
> #####  [itrace 命令](https://github.com/dsw0214/linux-commands/blob/master/itrace.md "itrace 命令") : 命令会跟踪进程的库函数调用，它会显示出哪个库函数被调用

###  有关磁盘与文件系统的命令
> #####  [mount 命令](https://github.com/dsw0214/linux-commands/blob/master/mount.md "mount 命令") : 挂载文件系统
> #####  [umount 命令](https://github.com/dsw0214/linux-commands/blob/master/umount.md "umount 命令") : 卸载文件系统
> #####  [fsck 命令](https://github.com/dsw0214/linux-commands/blob/master/fsck.md "fsck 命令") : 检查并修复 Linux文件系统转换或复制文件
> #####  [dumpe2fs 命令](https://github.com/dsw0214/linux-commands/blob/master/dumpe2fs.md "dumpe2fs 命令") : 导出ext2/ext3/ext4文件系统信息
> #####  [dump 命令](https://github.com/dsw0214/linux-commands/blob/master/dump.md "dump 命令") : ext2/3/4文件系统备份工具
> #####  [fdisk 命令](https://github.com/dsw0214/linux-commands/blob/master/fdisk.md "fdisk 命令") : 磁盘分区命令,适用于2TB以下磁盘分区
> #####  [parted 命令](https://github.com/dsw0214/linux-commands/blob/master/parted.md "parted 命令") : 磁盘分区命令,没有磁盘大小限制,常用于2TB以下磁盘分区
> #####  [mkfs 命令](https://github.com/dsw0214/linux-commands/blob/master/mkfs.md "mkfs 命令") : 格式化创建 Linux文件系统
> #####  [partprobe 命令](https://github.com/dsw0214/linux-commands/blob/master/partprobe.md "partprobe 命令") : 更新内核的硬盘分区表信息
> #####  [e2fsck 命令](https://github.com/dsw0214/linux-commands/blob/master/e2fsck.md "e2fsck 命令") : 检查ext2/ext3/ext4类型文件系统
> #####  [mkswap 命令](https://github.com/dsw0214/linux-commands/blob/master/mkswap.md "mkswap 命令") : 创建 Linux交换分区
> #####  [swapon 命令](https://github.com/dsw0214/linux-commands/blob/master/swapon.md "swapon 命令") : 启用交换分区
> #####  [swapoff 命令](https://github.com/dsw0214/linux-commands/blob/master/swapoff.md "swapoff 命令") : 关闭交换分区
> #####  [sync 命令](https://github.com/dsw0214/linux-commands/blob/master/sync.md "sync 命令") : 将内存缓冲区内的数据写入磁盘
> #####  [resize2fs 命令](https://github.com/dsw0214/linux-commands/blob/master/resize2fs.md "resize2fs 命令") : 调整ext2/ext3/ext4文件系统大小

###  文件压缩及解压缩命令
> #####  [tar 命令](https://github.com/dsw0214/linux-commands/blob/master/tar.md "tar 命令") : 打包压缩
> #####  [unzip 命令](https://github.com/dsw0214/linux-commands/blob/master/unzip.md "unzip 命令") : 解压文件
> #####  [gzip 命令](https://github.com/dsw0214/linux-commands/blob/master/gzip.md "gzip 命令") : gzip压缩工具
> #####  [bzip2 命令](https://github.com/dsw0214/linux-commands/blob/master/bzip2.md "bzip2 命令") : bzip2压缩工具
> #####  [zip 命令](https://github.com/dsw0214/linux-commands/blob/master/zip.md "zip 命令") : 压缩工具

###  查看文件及内容处理命令
> #####  [cat 命令](https://github.com/dsw0214/linux-commands/blob/master/cat.md "cat 命令") : 全拼concatenate,功能是用于连接多个文件并且打印到屏幕输出或重定向到指定文件中
> #####  [tac 命令](https://github.com/dsw0214/linux-commands/blob/master/tac.md "tac 命令") : tac是cat的反向拼写,因此命令的功能为反向显示文件内容
> #####  [more 命令](https://github.com/dsw0214/linux-commands/blob/master/more.md "more 命令") : 分页显示文件内容
> #####  [less 命令](https://github.com/dsw0214/linux-commands/blob/master/less.md "less 命令") : 分页显示文件内容,more命令的相反用法
> #####  [head 命令](https://github.com/dsw0214/linux-commands/blob/master/head.md "head 命令") : 显示文件内容的头部
> #####  [tail 命令](https://github.com/dsw0214/linux-commands/blob/master/tail.md "tail 命令") : 显示文件内容的尾部
> #####  [cut 命令](https://github.com/dsw0214/linux-commands/blob/master/cut.md "cut 命令") : 将文件的每一行按指定分隔符分割并输出
> #####  [split 命令](https://github.com/dsw0214/linux-commands/blob/master/split.md "split 命令") : 分割文件为不同的小片段
> #####  [paste 命令](https://github.com/dsw0214/linux-commands/blob/master/paste.md "paste 命令") : 按行合并文件内容
> #####  [sort 命令](https://github.com/dsw0214/linux-commands/blob/master/sort.md "sort 命令") : 对文件的文本内容排序
> #####  [uniq 命令](https://github.com/dsw0214/linux-commands/blob/master/uniq.md "uniq 命令") : 去除重复行 oldboy
> #####  [wc 命令](https://github.com/dsw0214/linux-commands/blob/master/wc.md "wc 命令") : 统计文件的行数、单词数或字节数
> #####  [iconv 命令](https://github.com/dsw0214/linux-commands/blob/master/iconv.md "iconv 命令") : 转换文件的编码格式
> #####  [dos2unix 命令](https://github.com/dsw0214/linux-commands/blob/master/dos2unix.md "dos2unix 命令") : 将DOS格式文件转换成UNIX格式
> #####  [diff 命令](https://github.com/dsw0214/linux-commands/blob/master/diff.md "diff 命令") : 全拼 difference,比较文件的差异,常用于文本文件
> #####  [vimdiff 命令](https://github.com/dsw0214/linux-commands/blob/master/vimdiff.md "vimdiff 命令") : 命令行可视化文件比较工具,常用于文本文件
> #####  [rev 命令](https://github.com/dsw0214/linux-commands/blob/master/rev.md "rev 命令") : 反向输出文件内容
<<<<<<< HEAD
> #####  [grep 命令](https://github.com/dsw0214/linux-commands/blob/master/grep.md "grep 命令"): 过滤字符串,三剑客老三
=======
[grep 命令](https://github.com/dsw0214/linux-commands/blob/master/grep.md "grep 命令"): 过滤字符串,三剑客老三
>>>>>>> 81625cb26f836501915bef8e023c2d4063b1cc33
> #####  [egrep 命令](https://github.com/dsw0214/linux-commands/blob/master/egrep.md "egrep 命令") : 过滤字符串,三剑客老三
> #####  [join 命令](https://github.com/dsw0214/linux-commands/blob/master/join.md "join 命令") : 按两个文件的相同字段合并
> #####  [tr 命令](https://github.com/dsw0214/linux-commands/blob/master/tr.md "tr 命令") : 替换或删除字符
> #####  [vi 命令](https://github.com/dsw0214/linux-commands/blob/master/vi.md "vi 命令"): 命令行文件编辑器
> #####  [vim 命令](https://github.com/dsw0214/linux-commands/blob/master/vim.md "vim 命令") : 命令行文件编辑器
> #####  [sed 命令](https://github.com/dsw0214/linux-commands/blob/master/sed.md "sed 命令") : 一种流编编器
> #####  [awk 命令](https://github.com/dsw0214/linux-commands/blob/master/awk.md "awk 命令") : 一种行处理器

###  搜索文件命令
> #####  [which 命令](https://github.com/dsw0214/linux-commands/blob/master/which.md "which 命令") : 查找二进制命令,按环境变量PATH路径查找
> #####  [find 命令](https://github.com/dsw0214/linux-commands/blob/master/find.md "find 命令") : 从磁盘遍历查找文件或目录
> #####  [whereis 命令](https://github.com/dsw0214/linux-commands/blob/master/whereis.md "whereis 命令") : 查找二进制命令,按环境变量PATH路径查找
> #####  [locate 命令](https://github.com/dsw0214/linux-commands/blob/master/locate.md "locate 命令") : 从数据库(var/lib/locate/locate.db)查找命令,使用updated更新库

###  查看系统用户登陆信息的命令
> #####  [whoami 命令](https://github.com/dsw0214/linux-commands/blob/master/whoami.md "whoami 命令") : 显示当前有效的用户名称,相当于执行id-un命令
> #####  [who 命令](https://github.com/dsw0214/linux-commands/blob/master/who.md "who 命令") : 显示目前登录系统的用户信息
> #####  [w 命令](https://github.com/dsw0214/linux-commands/blob/master/w.md "w 命令") : 显示已经登陆系统的用户列表,并显示用户正在执行的指令
> #####  [last 命令](https://github.com/dsw0214/linux-commands/blob/master/last.md "last 命令") : 显示登入系统的用户
> #####  [lastlog 命令](https://github.com/dsw0214/linux-commands/blob/master/lastlog.md "lastlog 命令") : 显示系统中所有用户最近一次登录信息
> #####  [users 命令](https://github.com/dsw0214/linux-commands/blob/master/users.md "users 命令") : 显示当前登录系统的所有用户的用户列表
> #####  [finger 命令](https://github.com/dsw0214/linux-commands/blob/master/finger.md "finger 命令") : 查找并显示用户信息

###  深入网络操作命令
> #####  [nmap 命令](https://github.com/dsw0214/linux-commands/blob/master/nmap.md "nmap 命令") : 网络扫描命令
> #####  [lsof 命令](https://github.com/dsw0214/linux-commands/blob/master/lsof.md "lsof 命令") : 全名list open files,也就是列举系统中已经被打开的文件
> #####  [mail 命令](https://github.com/dsw0214/linux-commands/blob/master/mail.md "mail 命令") : 发送和接收邮件
> #####  [mutt 命令](https://github.com/dsw0214/linux-commands/blob/master/mutt.md "mutt 命令") : 邮件管理命令
> #####  [nslookup 命令](https://github.com/dsw0214/linux-commands/blob/master/nslookup.md "nslookup 命令") : 交互式查询互联网DNS服务器的命令
> #####  [dig 命令](https://github.com/dsw0214/linux-commands/blob/master/dig.md "dig 命令") : 查找DNS解析过程
> #####  [host 命令](https://github.com/dsw0214/linux-commands/blob/master/host.md "host 命令") : 查询DNS的命令
> #####  [traceroute 命令](https://github.com/dsw0214/linux-commands/blob/master/traceroute.md "traceroute 命令") : 追踪数据传输路由状况
> #####  [tcpdump 命令](https://github.com/dsw0214/linux-commands/blob/master/tcpdump.md "tcpdump 命令") : 命令行抓包工具

###  内置命令及其它
> #####  [echo 命令](https://github.com/dsw0214/linux-commands/blob/master/echo.md "echo 命令") : 打印变量,或直接输出指定的字符串
> #####  [printf 命令](https://github.com/dsw0214/linux-commands/blob/master/printf.md "printf 命令") : 将结果格式化输出到标准输出
> #####  [rpm 命令](https://github.com/dsw0214/linux-commands/blob/master/rpm.md "rpm 命令") : 管理rpm包的命令
> #####  [yum 命令](https://github.com/dsw0214/linux-commands/blob/master/yum.md "yum 命令") : 自动化简单化地管理rpm包的命令
> #####  [watch 命令](https://github.com/dsw0214/linux-commands/blob/master/watch.md "watch 命令") : 周期性的执行给定的命令,并将命令的输出以全屏方式显示
> #####  [alias 命令](https://github.com/dsw0214/linux-commands/blob/master/alias.md "alias 命令") : 设置系统别名
> #####  [unalias 命令](https://github.com/dsw0214/linux-commands/blob/master/unalias.md "unalias 命令") : 取消系统别名
> #####  [date 命令](https://github.com/dsw0214/linux-commands/blob/master/date.md "date 命令") : 查看或设置系统时间
> #####  [clear 命令](https://github.com/dsw0214/linux-commands/blob/master/clear.md "clear 命令") : 清除屏幕,简称清屏
> #####  [history 命令](https://github.com/dsw0214/linux-commands/blob/master/history.md "history 命令") : 查看命令执行的历史纪录
> #####  [eject 命令](https://github.com/dsw0214/linux-commands/blob/master/eject.md "eject 命令") : 弹出光驱
> #####  [time 命令](https://github.com/dsw0214/linux-commands/blob/master/time.md "time 命令") : 计算命令执行时间
> #####  [nc 命令](https://github.com/dsw0214/linux-commands/blob/master/nc.md "nc 命令") : 功能强大的网络工具
> #####  [xargs 命令](https://github.com/dsw0214/linux-commands/blob/master/xargs.md "xargs 命令") : 一种管道命令
> #####  [export 命令](https://github.com/dsw0214/linux-commands/blob/master/export.md "export 命令") : 设置或者显示环境变量
> #####  [unset 命令](https://github.com/dsw0214/linux-commands/blob/master/unset.md "unset 命令") : 删除变量或函数
> #####  [type 命令](https://github.com/dsw0214/linux-commands/blob/master/type.md "type 命令") : 用于判断另外一个命令是否是内置命令
> #####  [bc 命令](https://github.com/dsw0214/linux-commands/blob/master/bc.md "bc 命令") : 命令行科学计算器

###  关机:重启:注销和查看系统信息的命令
> #####  [shutdown 命令](https://github.com/dsw0214/linux-commands/blob/master/shutdown.md "shutdown 命令") : 关机
> #####  [halt 命令](https://github.com/dsw0214/linux-commands/blob/master/halt.md "halt 命令") : 关机
> #####  [poweroff 命令](https://github.com/dsw0214/linux-commands/blob/master/poweroff.md "poweroff 命令") : 关闭电源
> #####  [logout 命令](https://github.com/dsw0214/linux-commands/blob/master/logout.md "logout 命令") : 退出当前登录的She11
> #####  [exit 命令](https://github.com/dsw0214/linux-commands/blob/master/exit.md "exit 命令") : 退出当前登录的She11

###  基础网络操作命令
> #####  [telnet 命令](https://github.com/dsw0214/linux-commands/blob/master/telnet.md "telnet 命令") : 使用telnet协议远程登录
> #####  [ssh 命令](https://github.com/dsw0214/linux-commands/blob/master/ssh.md "ssh 命令") : 使用SSH加密协议远程登录
> #####  [scp 命令](https://github.com/dsw0214/linux-commands/blob/master/scp.md "scp 命令") : 全拼 secure copy,用于不同主机之间复制文件
> #####  [wget 命令](https://github.com/dsw0214/linux-commands/blob/master/wget.md "wget 命令") : 命令行下载文件
> #####  [ping 命令](https://github.com/dsw0214/linux-commands/blob/master/ping.md "ping 命令") : 测试主机之间网络的连通性
> #####  [route 命令](https://github.com/dsw0214/linux-commands/blob/master/route.md "route 命令") : 显示和设置 linux系统的路由表
> #####  [ifconfig 命令](https://github.com/dsw0214/linux-commands/blob/master/ifconfig.md "ifconfig 命令") : 查看配置、启用或禁用网络接口的命令
> #####  [ifup 命令](https://github.com/dsw0214/linux-commands/blob/master/ifup.md "ifup 命令") : 启动网卡
> #####  [ifdown 命令](https://github.com/dsw0214/linux-commands/blob/master/ifdown.md "ifdown 命令") : 关闭网卡
> #####  [netstat 命令](https://github.com/dsw0214/linux-commands/blob/master/netstat.md "netstat 命令") : 查看网络状态
> #####  [ss 命令](https://github.com/dsw0214/linux-commands/blob/master/ss.md "ss 命令") : 命令行查看网络


## Contributing workflow (参与工作流)

以下是我建议您对该项目进行更改的方法：
1. [FORK THIS PROJECT](https://help.github.com/articles/fork-a-repo/ "FORK THIS PROJET") TO YOUR ACCOUNT.
2. [CREATE A BRANCH](https://help.github.com/articles/creating-and-deleting-branches-within-your-repository "CREATE A BRANCH") FOR THE CHANGE YOU INTEND TO MAKE.
3. MAKE YOUR CHANGES TO YOUR FORK.
4. [SEND A PULL REQUEST](https://help.github.com/articles/using-pull-requests/ "SEND A PULL REQUEST") FROM YOUR FORK’S BRANCH TO OUR MASTER BRANCH.

使用基于Web的界面进行更改也很好，并且通过自动分叉项目和提示发送请求来帮助您。

## License
- ##### [The MIT License](https://github.com/dsw0214/linux-commands/blob/master/LICENSE "The MIT License")
> **欢迎任何人参与和完善：一个人可以走的很快，但是一群人却可以走的更远**

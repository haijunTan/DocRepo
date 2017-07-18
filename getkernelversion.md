# 查看linux版本信息的几种方法

## 1.在命令行输入uname -a可以查看内核版本详细信息，其中包括主机名称。
'''
uname -a
vagrant@homestead:~$ uname -aLinux homestead 3.13.0-24-generic #47-Ubuntu SMP Fri May 2 23:30:00 UTC 2014 x86_64 x86_64 x86_64 GNU/Linux
'''

## 2.在命令行输入"cat /proc/version",说明正在运行的内核版本。
'''
cat /proc/version
vagrant@homestead:~$ cat /proc/versionLinux version 3.13.0-24-generic (buildd@batsu) (gcc version 4.8.2 (Ubuntu 4.8.2-19ubuntu1) ) #47-Ubuntu SMP Fri May 2 23:30:00 UTC 2014
'''


## 3.在命令行输入"cat /etc/issue", 显示的是发行版本信息
'''
cat /etc/issue
vagrant@homestead:~$ cat /etc/issueUbuntu 14.04.2 LTS \n \l
'''

## 4.FSG（Free Standards Group）组织开发的LSB (Linux Standard Base)标准的一个命令，用来查看linux兼容性的发行版信息。适用于所有的linux，包括Redhat、SuSE、Debian等发行版，但是在debian下要安装lsb
'''
lsb_release -a
vagrant@homestead:~$ lsb_release -aNo LSB modules are available.Distributor ID:    UbuntuDescription:    Ubuntu 14.04.2 LTSRelease:    14.04Codename:    trusty
'''

#### apache-users软件包描述

这个[Perl](https://www.perl.org/)脚本会枚举使用了[UserDir模块](https://httpd.apache.org/docs/2.4/mod/mod_userdir.html)的[Apache](https://httpd.apache.org/)服务器的系统的用户名。  
[apache-users Homepage](https://labs.portcullis.co.uk/) | [Kali apache-users Repo](http://git.kali.org/gitweb/?p=packages/apache-users.git;a=summary)

* Author: Andy@Portcullis
* License: GPLv2

##### 包含在apache-users包中的工具

> apache-users - 枚举含有Apache服务器UserDir模块的系统中的用户名
```bash
root@kali： apache-users
USAGE: apache-users [-h 1.2.3.4] [-l names] [-p 80] [-s (SSL Support 1=true 0=false)] [-e 403 (http code)] [-t threads]
```

##### apache-users使用示例

指定远程主机(-h 192.168.1.202), 传递一个包含用户名的文件夹(-l /usr/share/wordlists/metasploit/unix_users.txt), 指定端口号(-p 80), 禁用ssl(-s 0), 指定http错误代码(-e 403), 使用的线程数(-t 10)
```bash
root@kali:~# apache-users -h 192.168.1.202 -l /usr/share/wordlists/metasploit/unix_users.txt -p 80 -s 0 -e 403 -t 10
```
原文链接: [https://tools.kali.org/web-applications/apache-users](https://tools.kali.org/web-applications/apache-users)

译者: xiiiAtCn  
校对:
## Linux command
command _\[options][arguments]_

options: 怎么做， arguments:对谁做 </br>

**_请不要使用这个命令_！** ：sudo rm -rf /* </br>
-rf 强制删除

### 1. 文件和目录操作 
目录指代 : （1）. 是当前路径，(2) ~ 用户目录, (3) ../ 上一级目录，(4) ../ 上上一级目录 </br>

**文件路径**：</br>
- /etc 
- ls -F  可区分文件与文件夹

**通配符：**
- \* 任意everything </br>
- ? 单个字符，可寻未知的字，如: ls mor? </br>
- [  ] 括号里可选一个， 如：\[0-9][a-z] </br>
- { } 多个，如：ls {*.conf, *.cfg} </br>

### 文件命令
- ls, cd, pwd, cp (复制), find (指定目录查找文件)，mkdir (make directory),rmdir, mv (改名或移动) , rm (remove), touch (创建或更新)
- 如：find /usr/local -name "your.ini"

### 文件内容命令
- vi / vim : 编辑文本文件： _Shift + G_ jump to final，/ 查找内容， _n_ 下一处，_:1_ jump to first line，_:q!_ 放弃修改，_:wq_ 保存，_i_ to edit, _Esc_退出
- cat 拼接后输出内容, more, less, tail, 如：可看动态新日志： tail -f .conf 
- grep 过滤文本内容, 如：ps -ef | grep mysql， grep -i bind redis.conf 在redis.conf里找bind 
- \>  输出重定向， >> 追加或写入， 如: find /etc/ -name "*.conf" > new.txt

### 文件压缩命令
- tar
- tar -xzvf
-n tar -cvf file.tar redis-6-1 ： 打包redis6-2-1成file.tar
### 用户管理 
- groupadd, groupdel, useradd, userdel, passwd, su, sudo, chmod , chown
- 权限： drwxrw-rw- :
  - directory/file/link, owner, groups, others </br>
r,read = 4 , w,write=2, x,execute=1 </br>
chmod 700 file.txt </br>
### 网络命令
- ping 测试网络连通性
- ifconfig 查看网络
- telnet 远程连接
- wget 下载， 列如：wget https://xxx.com
- nestat 查看网络状态
### 系统状态
- df (disk file) ：查看磁盘使用情况
- top  : 查看系统资源使用情况
- ps (processes) : 查看进程状态, 如：ps -ef
- kill : 杀死进程
- free : 查看系统内存, 如：free -m
- date : 查看系统时间
- 查看系统操作系统版本：
  - n cat /proc/version
  - uname -a
  - lsb_release -a
- **启动服务：**
  - service mysql start
  - service mysql stop
  - service mysql restart
  - service mysql status
  - service apache2 start
  - /etc/init.d/nginx start
- **deb安装包：**
  - install : dpkg -i deb sogoupinyin.deb
  - delete : dpkg -e sogoupinyin.deb
- **apt安装：**
  - apt search xxx
  - apt install xxx

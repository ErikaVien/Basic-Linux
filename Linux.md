<h1>Linux</h1> 

ls, pwd, file, cp, whereis, which, locate, mkdir, mv, rm, touch, find, mount

-i (inquiry) 
-v (verbose)
-f (force)
-r (recursion)
-p (perents)

mkdir /sdb-u
mount /dev/sdb1/sdb-u

File compression/decompression
command line : tar, zip, unzip

Redhat - Redhat, CenOS, Fedora - make, rpm, yum, dnf
Debian - Kali, Ubuntu - deb, apt, dpkg
FreeBSD - FreeBSD - make, pkg, ports

rpm (RedHat Package Manager) - cannot resolve software dependencies, will cause error if one of dependencies is uninstall
yum (Yellow dog Updater) - resolve software dependencies 
DNF - Dandified YUM , updated form of yum

apt and yum is similiar
rpm, deb no use
Debian : apt search, apt install, apt update, apt remove
FreeBSD : pkg search, pkg install, pkg upgrade, pkd del

update-alternative - software version manager

Managing user/group

cat /etc/group - check group list
groups - check user group
groupadd security - add group
groupdel security - delete group
useradd - add user
passwd - change user passw
userdel - delete user
usermod - change user info

wget - only support http, https
scp - secure copy
curl - more informative than wget

Linux system display setting
check time/date - date, cal, uptime
display sys version : uname -a , cat /proc/version
display task processes : systemctl list-unit-files

ps (process status)
-a : list all process
-u :
-x :
-e : list all process
-f : display in detail, use with -e -> ps -ef

Service control
systemctl status *.service
systemctl start mysqld.service
restart, stop, 
systemctl enable mysqld.service
systemctl disable mysqld.service 

free -h : display internal storage
du (disk usage)
sar (system activity reporter)

Task Automation
tools : crontab
https://tool.lu/crontab

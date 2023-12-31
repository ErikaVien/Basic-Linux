## Linux file system 目录结构
- **_/root_** : the home directory of all-powerful root user 超级用户目录
- **_/etc_** : contains linux configuration files that control when and how programs start up 系统配置文件
- **_/bin_** : where application binaries reside 存放二进制可执行文件
- **_/sbin_**: contains system binaries files which only executables by system administration 存放可执行的文件，只有root能访问
- **_/home_** : user's home directory 用户文件的根目录
- _**/dev**_ : special device files 存放设备文件
- _**/lib**_ : libraries (shared program that are similiar to windows DLLs) 存放根文件系统中的程序运行所需的共享库及内核模块
- _**/media**_ : USB, CDs devices mounted 移除性媒体
- _**/mnt**_ : where other file systems mounted to filesystem 系统管理员安装临时文件系统的安装点
- _**/opt**_ :optional files reserved for the installation of add-on application software packages 附加的应用程序软件包
- _**/proc**_ : view of internal kernel data 开机生成，关机自动消失
- _**/srv**_ : site-specific data, service 存放一些服务启动之后要提取的数据
- _**/sys**_ : contains information from devices connected to your computer 文件系统相关文件
- _**/tmp**_ : store temporary directories 临时各种文件
- _**/usr**_ :  contains shareable, read-only commands, libraries, and data 存放共享的系统资源
- _**/var**_ : variable data files 运行时需要改变数目的文件, 如：log files, spool files and cache files
- _**/boot**_ : contains the static bootloader and kernel executable and configuration files required to boot 启动

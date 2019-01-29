```
pacman -Sy 仅同步源
pacman -Syu 同步源，并更新系统
pacman -Su --ignore foo 升级时不升级包foo
pacman -S abc 从本地数据库中得到abc的信息，下载安装abc包
pacman -Sy abc 和源同步后安装名为abc的包
pacman -Sd abc 忽略依赖性问题，安装包abc
pacman -Sf abc 强制安装包abc
pacman -Si abc 从数据库中搜索包abc的信息
pacman -Ss abc 搜索有关abc信息的包
pacman -Sg abc 查询abc这个包组包含的软件包
pacman -Sw abc 下载包而不安装它
pacman -R abc 删除abc包
pacman -Rc abc 删除abc包和依赖abc的包
pacman -Rsn abc 删除包所有不需要的依赖包并删除其配置文件
pacman -Rscn abc 删除abc包所有不需要的依赖包和依赖abd的包并删除其配置文件
pacman -Sc 清理/var/cache/pacman/pkg目录下的旧包
pacman -Scc 清除所有下载的包和数据库
pacman -Q 列出系统中所有的包
pacman -Q package 在本地包数据库搜索(查询)指定软件包
pacman -Qi package 在本地包数据库搜索(查询)指定软件包并列出相关信息
pacman -Q | wc -l 统计当前系统中的包数量
pacman -Qdt 找出孤立包
pacman -Rns $(pacman -Qtdq) 删除孤立软件包（递归的,小心用)
pacman -U abc.pkg.tar.gz 安装下载的abs包，或新编译的本地abc包
pacman-optimize && sync 提高数据库访问速度
```

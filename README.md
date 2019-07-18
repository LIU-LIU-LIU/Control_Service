# Control_Service
## 这个脚本是在linux做的一个类似systemctl的简单脚本，用来控制服务<br>  
## For Linux<br>
## By liu.liuy@qq.com<br>

功能：
操作类似systemctl
./Control_Service [选项] [参数]
./Control_Service	不填写选项进入主程序，互动模式

[选项]:
-h/--help	查看帮助
start	启动服务 
stop	停止服务
status	查看服务状态，在pid或者port指定的情况下可以使用
restart	重启服务
reload	重新加载服务，指定的情况下可以使用
enable	添加服务到开机自启
disable	从开机自启中删除，在添加过开机自启的情况下使用。

使用:
1.下载Control_Service
2.chmoe +x Control_Service	添加运行权限
3../Control_Service	运行此程序
4../Control_Service --help或者./Control_Service进入后输入4查看帮助

文件:
Control_Service		主程序,可以添加到环境变量在任何目录调用。
Control_Service.conf	配置文件,启动程序时自动创建。
/etc/rc.d/rc.local	会修改此文件，以达到开机自启的功能。

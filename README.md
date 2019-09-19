# Control_Service
## 这个脚本是在linux做的一个类似systemctl的简单脚本，用来控制服务<br>  
## For Linux<br>
## By liu.liuy@qq.com<br>

功能：<br>
操作类似systemctl<br>
./Control_Service [选项] [参数]<br>
./Control_Service	不填写选项进入主程序，交互模式<br>
<br>
[选项]:<br>
-h/--help	查看帮助<br>
start	启动服务 <br>
stop	停止服务<br>
status	查看服务状态，在pid或者port指定的情况下可以使用<br>
restart	重启服务<br>
reload	重新加载服务，指定的情况下可以使用<br>
enable	添加服务到开机自启<br>
disable	从开机自启中删除，在添加过开机自启的情况下使用。<br>
<br>
使用:<br>
1.下载Control_Service<br>
2.chmoe +x Control_Service	添加运行权限<br>
3../Control_Service	运行此程序<br>
4../Control_Service --help或者./Control_Service进入后输入4查看帮助<br>
<br>
文件:<br>
Control_Service		主程序,可以添加到环境变量在任何目录调用。<br>
Control_Service.conf	配置文件,启动程序时自动创建。<br>
/etc/rc.d/rc.local	会修改此文件，以达到开机自启的功能。<br>
<br>

![Image text](https://liuliuliu.club:88/test/%E6%8E%A7%E5%88%B6%E6%9C%8D%E5%8A%A1%E6%88%AA%E5%9B%BE.png)
功能截图<br>

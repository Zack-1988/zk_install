本脚本可配置不限制服务器台数的zookeeper和kafka服务，并将于脚本获取的最后一台服务器上安装可视化web管理界面。

使用方法：
bash zk_install.sh

请输入本次要配置zookeeper/kafka的服务器数量：x
请输入服务器1的ip地址:192.168.0.1
...
请输入服务器x的ip地址:192.168.0.x
。。。
。。。
。。。
--------------安装已完成----------------
WEB管理界面地址为：192.168.0.x:8048/ke
---------------感谢使用-----------------


注：
zookeeper与kafka需依赖于java环境，若生产环境已安装java环境，版本不兼容将导致服务无法启动；
可视化web管理界面需要更多内存，否则将导致服务启动失败，无法创建topic等；
本脚本使用了pdsh工具，工具下载可在 https://github.com/RbClimber/pdsh 下载。

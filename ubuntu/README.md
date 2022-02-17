# 服务器重启，重新打开应用
code-server(code-server)

nacos(ubuntu):path/start-nacos.sh

redis(ubuntu):service redis start

rocketMQ(code-server):nohup sh bin/mqnamesrv &  |  nohup sh mqbroker -n localhost:9876 -c ../conf/broker.conf &   (记得切jdk版本到8以下)

mysql(ubuntu):service mysql start

crondtab: service cron start

qqbot

# nano
crtl+x 

crtl+o 保存

# screen

ctrl+a+d    |不关闭screen退出
exit        |关闭screen

# update-alternatives
update-alternatives --config java 可以用来切换java版本，管理java版本号

update-alternatives --install <链接> <名称> <路径> <优先级>  用来加入版本信息

# netstat -ntlp 查看端口监听情况

# free -m 查看内存使用情况

# echo 3 > /proc/sys/vm/drop_caches 清除缓存

# ifconfig 查看网卡配置信息

# screen 进入attached状态的screen
screen -D  -r ＜session-id>

-D -r  先踢掉前一用户，再登陆。

# statnet -ntl 查看服务监听端口情况
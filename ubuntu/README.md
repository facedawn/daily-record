# 服务器重启，重新打开应用
code-server(code-server)
nacos(ubuntu):path/start-nacos.sh
redis(ubuntu):service redis start
rocketMQ(code-server):nohup sh bin/mqnamesrv &  |  nohup sh bin/mqbroker -n localhost:9876 &
mysql(ubuntu):service mysql start
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
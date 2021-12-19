不能用jdk8以上的版本跑

nohup sh mqnamesrv & 

nohup sh mqbroker -n localhost:9876 &
(指定使用broker.conf配置跑:nohup sh mqbroker -n localhost:9876 -c ../conf/broker.conf &)

sh mqshutdown broker/namesrv

初始设置在使用时会有问题，得在conf/broker.conf中添加
namesrvAddr=xx.xx.xx.xx:9876
brokerIP1=xx.xx.xx.xx
才能使用
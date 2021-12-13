不能用jdk8以上的版本跑

nohup sh mqnamesrv &

nohup sh mqbroker -n localhost:9876 &

sh shutdown.sh broker/namesrv
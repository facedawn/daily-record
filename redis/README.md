redis设置密码：config set requirepass 123456   （重启后失效）
或者修改 /etc/redis.conf 中的requirepass值 （永久生效）

/etc/redis/redis.conf 内部配置绑定ip（默认127.0.0.1，换成0.0.0.0可以全局监听）
也可以配置密码

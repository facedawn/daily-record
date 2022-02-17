# 查看表结构：
desc [表名]

# 查看所有用户：
SELECT user FROM mysql.user;

# mysql区分大小写(Linux系统下mysql8.0默认大小写敏感)
打开该mysql数据库的配置文件my.cnf

在my.cnf中的[mysqld]下,添加

lower_case_table_names = 1

1表示不区分大小写，0区分大小写
（8.0需要更复杂的配置 https://blog.csdn.net/baidu_36528788/article/details/119893596）
SHOW VARIABLES where Variable_name like 'lower%';查看是否修改正确

# 重置自增id
truncate 【tablename】

# java.sql.SQLNonTransientConnectionException: Public Key Retrieval is not allowed
在url的后边加上allowPublicKeyRetrieval=true
maven 跳过test进行install：

mvn clean install -DskipTests                      | 不执行测试，但会生成相应class文件

mvn clean install -Dmaven.test.skip=true           | 跳过测试的运行和编译//但windows系统下好像不能用，得用上面的

maven跑jar包出现no main class：

mvn exec:java -Dexec.mainClass="cn.xmu.classname"   |不带参数跑

mvn exec:java -Dexec.mainClass="cn.xmu.classname" -Dexec.args="arg0 arg1 arg2"  |带参数跑


# maven_jmeter_jenkins
step1：在eclipse中新建maven工程

step2：新建目录src/test/jmeter，拷贝jmter的项目jmx到该目录

step3：修改pom.xml，添加jmter-maven-plugin和jmeter-analysis-maven-plugin

step4：配置jenkins
![image](https://github.com/dongxiaobing/maven_jmeter_jenkins/blob/master/pic/jenkins_conf.jpg)

step5：运行结果
![image](https://github.com/dongxiaobing/maven_jmeter_jenkins/blob/master/pic/build_success.jpg)

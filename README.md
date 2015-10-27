# maven_jmeter_jenkins
step1：在eclipse中新建maven工程
step2：新建目录src/test/jmeter，拷贝jmter的项目jmx到该目录
step3：修改pom.xml
<build>
		<plugins>
			<plugin>
				<groupId>com.lazerycode.jmeter</groupId>
				<artifactId>jmeter-maven-plugin</artifactId>
				<version>1.10.1</version>
				<configuration>
					<resultsFileFormat>xml</resultsFileFormat>
					<ignoreResultFailures>true</ignoreResultFailures>
					<testResultsTimestamp>false</testResultsTimestamp>
				</configuration>
				<executions>
					<execution>
						<id>jmeter-tests</id>
						<phase>verify</phase>
						<goals>
							<goal>jmeter</goal>
						</goals>
					</execution>
				</executions>
			</plugin>
		</plugins>
	</build>

step4：配置jenkins
![image](https://github.com/dongxiaobing/maven_jmeter_jenkins/blob/master/pic/jenkins_conf.jpg)

step5：运行结果
![image](https://github.com/dongxiaobing/maven_jmeter_jenkins/blob/master/pic/jenkins_conf.jpg)

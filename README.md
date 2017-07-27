tomcat-redis-session-manager 
=======================================
---

tomcat版本
--------

支持tomcat8.5，没有对tomcat8.0、tomcat7做测试


用法
---
添加下面的配置到tomcat的context.xml中

    <Valve className="com.s.tomcat.redissessions.RedisSessionHandlerValve"/> 
	<Manager className="com.s.tomcat.redissessions.RedisSessionManager" 
			  host="192.168.10.162"
			  port="6379"
			  database="0" 
			  password="trj123456"
			  maxInactiveInterval="60" /> 



复制下面的文件到TOMCAT_BASE/lib目录:

- tomcat8.5-redis-session-manager.jar
- jedis-2.5.2.jar
- commons-pool2-2.2.jar

感谢
---
此版本修改自 https://github.com/jcoleman/tomcat-redis-session-manager


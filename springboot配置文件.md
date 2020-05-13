server :
  port : 8888
spring:
  datasource:
    #配置驱动
    driverClassName: com.mysql.cj.jdbc.Driver
    #数据库连接
    url: jdbc:mysql://127.0.0.1:3306/userdemo?useUnicode=true&characterEncoding=utf8&useSSL=false&serverTimezone=Asia/Shanghai&nullCatalogMeansCurrent=true
    #数据库的名称,biyi-form组件使用
    db-name: userdemo
    #数据库连接池
    #数据库用户名
    username: root
    #数据库密码
    password: Asdf1@34
    hikari:
      #最大连接池数
      maximumPoolSize: 20
    #是否自定义配置
    cachePrepStmts: true
    #连接池大小
    prepStmtCacheSize: 250
    #单条语句最大长度
    prepStmtCacheSqlLimit: 2048
    #新版本MySQL支持服务器端准备，是否开启
    useServerPrepStmts: true

mybatis:
  mapper-locations: classpath:mapper/*.xml
  configLocation: classpath:/mybatis-config.xml

   
   
   
   
mybatis-config.xml   
   
   <?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE configuration PUBLIC "-//mybatis.org//DTD Config 3.0//EN" "http://mybatis.org/dtd/mybatis-3-config.dtd"> 
<configuration> 
    <!-- 全局参数 --> 
	<settings>
		<!-- 设置但JDBC类型为空时,某些驱动程序要指定值,default:OTHER -->
		<setting name="jdbcTypeForNull" value="NULL"/> 
	</settings> 
</configuration>
   
   

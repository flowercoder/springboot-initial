server:
  port:8888
spring: 
   datasource: 
      #数据库驱动
      driverClassName: com.mysql.cj.jdbc.Driver
      #数据库连接
      url: jdbc:mysql://127.0.0.1:3306/managedb?useUnicode=true&characterEncoding=utf8&useSSL=false&serverTimezone=Asia/Shanghai&nullCatalogMeansCurrent=true
      #数据库的名称,biyi-form组件使用
      db-name: managedb
      #数据库连接池
      type: com.zaxxer.hikari.HikariDataSource
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

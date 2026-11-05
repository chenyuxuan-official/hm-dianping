# 黑马点评（hm-dianping）

基于 Spring Boot、MySQL、Redis 和 MyBatis-Plus 的本地生活点评项目学习代码。

## 环境配置

项目默认读取本地环境变量，避免把数据库和 Redis 密码写入仓库：

```text
DB_URL=jdbc:mysql://127.0.0.1:3306/hmdp?useSSL=false&serverTimezone=UTC&allowPublicKeyRetrieval=true
DB_USERNAME=root
DB_PASSWORD=你的数据库密码
REDIS_HOST=127.0.0.1
REDIS_PORT=6379
REDIS_PASSWORD=你的Redis密码
```

启动应用前配置这些环境变量即可。没有密码的 Redis 可将 `REDIS_PASSWORD` 留空。

## 启动

```bash
mvn spring-boot:run
```

默认服务端口：`8081`

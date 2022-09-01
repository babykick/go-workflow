## 依赖服务
### 启动redis
```
docker run -itd --name redis -p 6379:6379 redis
```

### 启动mysql
```
docker run -d -p 3306:3306 -it --name mysql -e MYSQL_ROOT_PASSWORD=123 mysql
```

## 开发
### go mod 化
```
go mod init workflow
go mod tidy -go=1.16 && go mod tidy -go=1.17
```
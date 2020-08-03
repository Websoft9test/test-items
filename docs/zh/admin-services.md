# 服务启停

使用由Websoft9提供的 Test 部署方案，可能需要用到的服务如下：

### Test

```shell
sudo systemctl start test-server
sudo systemctl stop test-server
sudo systemctl restart test-server
sudo systemctl status test-server

# you can use this debug mode if Test service can't run
test-server console
```

### MySQL

```shell
sudo systemctl start mysql
sudo systemctl stop mysql
sudo systemctl restart mysql
sudo systemctl status mysql
```

### Redis

```shell
systemctl start redis
systemctl stop redis
systemctl restart redis
systemctl status redis
```

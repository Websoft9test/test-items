# Start or Stop the Services

These commands you must know when you using the Test of Websoft9

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
sudo systemctl start redis
sudo systemctl stop redis
sudo systemctl restart redis
sudo systemctl status redis
```

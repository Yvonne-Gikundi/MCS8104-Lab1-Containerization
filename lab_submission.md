# Lab 1: Containerization - 152239

## 1. Docker command to create and run a container named `dbserver-mysql-nairobi`

Use the `customized-ubuntu:1.0` image to create a container named `dbserver-mysql-nairobi`. The command should map the container’s port 3306 to the host’s port 3309.

```dockerfile
Specify your commands here
docker run -it --name dbserver-mysql-nairobi -p 3309:3306 customized-ubuntu:1.0```

## 2. MySQL Server and MySQL Client Installation in Ubuntu

```shell
Specify your commands here
apt update
apt install -y mysql-server mysql-client
service mysql start 
mysql_secure_installation
```

## 3. Login using the MySQL Client and Change the MySQL Root Password

```sql
Specify your commands here
mysql -u root
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '5trathmore';
FLUSH PRIVILEGES;
EXIT;
```

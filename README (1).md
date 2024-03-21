
# Connection between RDS and EC2



## About Project

This project shows have to connect database created from RDS with EC2 instances. From this project we can access database created RDS with EC2 instance.

## Task

This project will follow following task:

- EC2 instance creation following above documentation
- RDS creation following above documentation
- Installation of mariadb in ec2 instance
- Establish connection between ec2 and mariadb with the help of endpoint. 



## Steps for installation of mariadb in EC2 instances

Update your system

```bash
  sudo apt update
```
 Install mariabd server

```bash
 sudo apt install mariadb-server
```
 Start mariadb server

```bash
  sudo systemctl start mariadb
```
 Enable mariadb server

```bash
  sudo systemctl enable mariadb
```
 Check the status of mariadb
```bash
  sudo systemctl status mariadb
```
 Connect to database server
```bash
  mysql -h <database-endpoint> -P 3306 -u admin -p
```
Now,we have access to mariadb database.
## Use Case

We can create databases through EC2 instance, make necessary changes through database. Also,we can access created databases.


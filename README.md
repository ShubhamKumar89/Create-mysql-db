# Create-mysql-db

## Login to your Server
```bash
ssh <ubuntu>@<ip> 
# e.g. ssh ubuntu@192.168.5.185
```

## Install mysql-server 
```bash
sudo apt-get install mysql-server
```

## Login to MYSQL monitor
```bash
sudo mysql -u root
```

## Create User
```bash
CREATE USER <db_username>@localhost IDENTIFIED BY '<password>';
# e.g. CREATE USER shubham@localhost IDENTIFIED BY 'password';
```

## Grant All Privileges
```bash
GRANT ALL PRIVILEGES ON *.* TO <db_username>@localhost;
# e.g. GRANT ALL PRIVILEGES ON *.* TO shubham@localhost;
```

## Exit MYSQL
```bash
\q
```

## Login back to MYSQL monitor
```bash
sudo mysql -u <db_username> -p
# e.g. sudo mysql -u shubham -p
```

## Create Database
```bash
CREATE DATABASE <database-name>;
# e.g. CREATE DATABASE sdb;
```

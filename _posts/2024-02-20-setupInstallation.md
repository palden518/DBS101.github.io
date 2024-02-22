---
title: Setup for SQL Practicals
sidebar:
  nav: pract-en
aside:
  toc: true
---

## Install PostgreSQL

[PostgreSQL Documentation for installation](https://www.postgresql.org/download/)

### Windows

[Download Installer](https://www.postgresql.org/download/windows/)

### Linux(Other OS)

Check if Postgresql is preinstalled
```javascript
 postgres --version
```
If the command is unrecognised install postgresql
```javascript
apt-get install postgresql-12
```

### For kali linux follow this blog 

[Install postgresql on Kali Linux](https://www.postgresql.r2schools.com/how-to-install-postgresql-on-kali-linux/)


### MacOS

```javascript
brew install postgresql@16
```
```javascript
echo export PATH="/opt/homebrew/opt/postgresql@16/bin:$PATH" >> ~/.zshrc
```
Check if Postgresql is installed successfully
```javascript
 postgres --version
```
Start server
```javascript
brew services start postgresql@<version you have installed>

Example: brew services start postgresql@16
```
Check if you can get into the server
```javascript
 psql postgres 
```
Quit server
```javascript
quit
```

### Test Commands

After installation test the following commands;


#### Windows

- Start server
  ```javascript
    net start postgresql-x64-<Version you have installed>

    Example: net start postgresql-x64-15
  ```
  OR

  ```javascript
    pg_ctl -D "C:\Program Files\PostgreSQL\<Version you have installed>\data" start

    Example: pg_ctl -D "C:\Program Files\PostgreSQL\15\data" start
  ```

#### Linux 

- Start Server
  
  Initialize Server
  ```javascript
  sudo service postgresql-<Version you have installed> initdb
  
  Example: sudo service postgresql-9.3 initdb
  ```
  Start server
  ```javascript
  sudo service postgresql-<Version you have installed> start

  Example: sudo service postgresql-9.3 start
  ```
  Log into server
  ```javascript
  sudo -u postgres psql
  ```
  Quit server
  ```javascript
  quit
  ```
### SQL Commands (Start the server and execute the following commands)
  - Create Database
  ```javascript
   CREATE DATABASE Demo
  ```
  - Create Table
  ```javascript
   CREATE TABLE student (
    StudentID int(8) NOT NULL,
    Name varchar(255),
    CID varchar(11) NOT NULL,
    programmeID varchar(5) NOT NULL,
    PRIMARY KEY (StudentID)
  );
  ```
  - Insert values into Table
  ```javascript
   INSERT INTO student (StudentID,Name,CID,programmeID) VALUES (02319987,'Pema Choden', '17828972541','BESWE')
  ```
   ```javascript
   INSERT INTO student (StudentID,Name,CID,programmeID) VALUES (02319917,'Tashi Tobgay', '178289724541','BEIT')
  ```
  #### Check constraints
  - Check constraints; Primary key
  ```javascript
   INSERT INTO student (StudentID,Name,CID,programmeID) VALUES (02319987,'Choden', '17818972541','BESWE')
  ```

  - Check constraints; NOT NULL
  ```javascript
   INSERT INTO student (StudentID,Name,CID,programmeID) VALUES (02319987,'Choden', ,'BESWE')
  ```

  - Check constraints; DATA TYPE Length
  ```javascript
   INSERT INTO student (StudentID,Name,CID,programmeID) VALUES (02319987,'Choden','182782782789728927' ,'BESWE')
  ```


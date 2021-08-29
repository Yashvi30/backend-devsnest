POSTGRES INSTALLATION

For linux
sudo -u postgres psql

psql (13.4 (Ubuntu 13.4-1.pgdg20.04+1))

```postgres=# CREATE USER username WITH PASSWORD 'password';
postgres=# CREATE DATABASE databasename;
postgres=# GRANT ALL PRIVILEGES ON DATABASE databasename TO username;
postgres=# GRANT SELECT PRIVILEGES ON DATABASE databasename TO username;
postgres=# GRANT INSERT PRIVILEGES ON DATABASE databasename TO username;
postgres=# GRANT DELETE PRIVILEGES ON DATABASE databasename TO username;
postgres=# GRANT UPDATE PRIVILEGES ON DATABASE databasename TO username;
postgres=# \c databasename [connect to database]

[AFTER CONNECTING TO DATABASE]

databasename=# CREATE TABLE tablename(
databasename(# ColumnName  DATATYPE NOT NULL,
databasename(# ColumnName  DATATYPE ,
databasename(# );
databasename=# \d [to display list of tables ]
databasename=# \d tablename [to display table properties]
databasename-# DROP TABLE tablename; [delete table]

postgres-# \l [all existing database can be seen]
postgres-# DROP DATABASE databasename; [delete database]
[first connect to different database then drop required database]
\q [to exit postgres]
```

```postgres=# CREATE SCHEMA schemaname;
postgres=# CREATE TABLE schemaname.tablename;[create table within schema]
DROP SCHEMA schemaname CASCADE; [to drop objects of schema and delete schema]
postgres=# INSERT INTO TABLENAME(COLUMNNAME1,COLUMNNAME2) VALUES ('1','2')[row1 data], ('3','4')[row2 data];[give values according to datatype][by default value NULL]
postgres=# SELECT * FROM TABLENAME;[to see data in table]

```

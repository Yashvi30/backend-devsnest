Redis Installation

For Linux

- Run the commands:
  > sudo apt-get install redis-server
  > sudo service redis-server restart
  > redis-cli

---

USAGE

- SET key value
- GET key
- ttl key
- KEYS \*
- DEL key
- FLUSHALL
- EXISTS key
- expire key time
- setex key time value

For Arrays

- LPUSH array value
- RPUSH array value
- LRANGE array start stop
- LPOP array
- RPOP array

For Sets

- SADD myset value
- SMEMBERS myset
- SREM myset value

For Object/Hash

- HSET key field value
- HGET key field
- HGETALL key
- HDEL key field
- HEXISTS key field

POSTGRES INSTALLATION

For linux
sudo -u postgres psql

psql (13.4 (Ubuntu 13.4-1.pgdg20.04+1))

postgres=# CREATE USER username WITH PASSWORD 'password';
postgres-# CREATE DATABASE databasename;
postgres-# GRANT ALL PRIVILEGES ON DATABASE databasename TO username;
postgres-# GRANT SELECT PRIVILEGES ON DATABASE databasename TO username;
postgres-# GRANT INSERT PRIVILEGES ON DATABASE databasename TO username;
postgres-# GRANT DELETE PRIVILEGES ON DATABASE databasename TO username;
postgres-# GRANT UPDATE PRIVILEGES ON DATABASE databasename TO username;
postgres-# \c databasename (connect to database)
postgres-# \l (all existing database can be seen)
postgres-# DROP DATABASE databasename; (delete database)

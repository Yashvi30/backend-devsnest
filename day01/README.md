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

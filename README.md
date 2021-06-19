# conoha-observer
Conoha comuputing observer.

# Refference
https://gist.github.com/3ng1n33r/428ba64aa9efa5b2261468578c46df61

# DR;TL;
## Stand up
```
docker-compose up
```

If it's happend to `zabbix-server exited with code 1`, you insert `create.sql` manually.
```sql
mysql> drop database K9brEwbDsdxtMyGAXV_zabbix;
mysql> create database K9brEwbDsdxtMyGAXV_zabbix;
mysql> ALTER DATABASE K9brEwbDsdxtMyGAXV_zabbix
    CHARACTER SET 'utf8'
    COLLATE 'utf8_bin'
;
```

```
mysql -u user_name -p zabbix_database < /path/to/create.sql
```
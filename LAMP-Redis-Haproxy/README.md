Playbook auto install LAMP + Redis and Haproxy on CentOS 7

About LAMP:
- Apache 2.4
- Mariadb 10.2
- PHP ver 7.2

Model:
```
       |
-------+-----------------------------------------------
       |
       +-------------------+--------------------+
       |[haproxy]          |[appserver-1]       |[appserver-2]
 +-----+-----+     +-------+------+     +-------+------+
 | Frontend  |     |   Backend#1  |     |   Backend#2  |
 |  HAProxy  |     |  Web Server  |     |  Web Server  |
 |           |     |  LAMP + Redis|     |  LAMP + Redis|
 +-----------+     +--------------+     +--------------+
```

Usage: `ansible-playbook -i hosts main.yml`

Note: file hosts You must edit match with Your puspose.

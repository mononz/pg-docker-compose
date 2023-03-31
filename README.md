PG w/ Docker
============

__First time run__

1. open docker on windows
2. In this dirctory run `docker volume create dbcult`
3. run `docker-compose up` in this directory
4. open pg admin and save a connections with the values, name= admin, host=localhost, port=5432, maintenanceDb=postgres, username=postgres, password=master_password
5. right click on admin, create login/group role. enter name=cultist, password=cultington and save
6. right click on admin, create database. enter database=cultist, select owner as cultist(the user/role from 5) and save.

__Development environment__

1. run `docker-compose up` in this directory (if not already running)
2. Your db connection in you client application should be host=localhost, user=cultist, password=cultington

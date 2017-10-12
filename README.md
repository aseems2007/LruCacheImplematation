# LruCacheImplematation
A simple Website with a cache implemented with LRU memory management technique. 

Pre Requisites:
-----------------------------------------------------------------------------
Latest version of the following installed and running. 

1. mySql Database
2. Apache Server running at local host. 
  If there is already a server running, you may need to change the port at which apache is listening. 
  It can be done at etc/apache2/ports.conf
  Add listen <Any Unutilized Port> 
  To find what ports are in use, use the command: #sudo netstat -tulpn

Database Setup:
---------------------------------------------------------------------------
Edit MySql username, Paswword, Database Name, Table Name in getMeaning.php 

- The Table need to contain two var char fields, One with the list of words and other with list of Meanings.
- For testing purpose, the cache is created with a size of 10, which can modified in lru.js file. lru.

Place the files, lru.js, getMeaning.php, index.php in /var/www/html folder. and run localhost at the set port. 
- If there is a problem in copying the files to /var/www/html folder, Access can be gained by using the command 
sudo nautilas. 

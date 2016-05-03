# nyc_pluto_mysql
Load NYC PLUTO dataset into MySQL database

Download PLUTO release 16v1 from http://www1.nyc.gov/site/planning/data-maps/open-data/dwn-pluto-mappluto.page
Unzip it. It'll create folder nyc_pluto_16v1.

Assumption:
You have a MySQL database user that can create a database.

Create a MySQL database:
<code>
  create database nyc;
  use nyc;
</code>

<code>
mysql -h <host> -u <mysql_user> -p<mysql_pwd> -D nyc
source pluto_16v1_load.sql
</code>



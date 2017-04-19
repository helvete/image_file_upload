# image_file_upload
Allow image file uploads, store link to filename relation in DB

How to make it run?

1/ Set up a virtual host at your web server
2/ Create a DB or just prepare the credentails to connect to it
3/ Copy `pdo_connect.php.sample` into `pdo_connect.php` and fill in DB connection credentials there

```
cp pdo_connect.php.sample pdo_connect.php
vi pdo_connect.php
```

4/ Create a new table structure - import db dump in ./scripts

```
mysql -u <db-user> -p <db-name> < ./scripts/uploader.sql
```

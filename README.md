This repository contains code that belongs to PhalconHosting.

--- This code is meant to be deployed only by the PhalconHosting master ---

[![Build Status](https://drone.io/github.com/Phalcon-hosting/phmaster/status.png)](https://drone.io/github.com/Phalcon-hosting/phmaster/latest)

Requirements
-------------

* Make sure to have phalcon extension loaded into php : ```php -m | grep phalcon```
* Make sure to have memcached server installed : ```service memcached status```
* Make sure to have memcache extension loaded into php : ```php -m | grep memcache```
* Make sure to have the pecl_http extension loaded into php (http://php.net/manual/en/http.install.php) : ```php -m | grep http```

Instaling
-------------


Run composer to install dependancies :

```
composer install
```


Copy the ```app/config/config.dist.php``` to ```app/config/config.php``` and update the content


Make the volt directory writtable by php
```
chown -R www-data app/cache #depends on which user will run the application
```

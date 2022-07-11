# Laravel/Lumen Docker Scaffold - Caprover

### **Description**

This will create a dockerized stack for a Laravel/Lumen application, consisted of the following containers:
-  **app**, your PHP application container

        Nginx, PHP8.1-fpm, Composer, NPM, Node.js v18.x


#### **Directory Structure**
```
+-- src <project root>
+-- configuration
|   +-- nginx
    |   +-- conf.d
        |   +-- app.conf
|   +-- php
    |   +-- local.ini
+-- lumen
|   +-- < Lumen files >
+-- .gitignore
+-- captain-definition
+-- docker-entry.sh
+-- Dockerfile
+-- docker-compose.yml
+-- readme.md <this file>
```


### **Setup instructions**

**Prerequisites:**

* Depending on your OS, the appropriate version of Docker Community Edition has to be installed on your machine.  ([Download Docker Community Edition](https://hub.docker.com/search/?type=edition&offering=community))


**Default configuration values**

The following values should be replaced in your `.env` file if you're willing to keep them as defaults:

    DB_HOST=mysql
    DB_PORT=3306
    DB_DATABASE=appdb
    DB_USERNAME=user
    DB_PASSWORD=myuserpass

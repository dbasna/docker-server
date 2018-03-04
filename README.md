# Docker Server Sample

## Preview
Provide an easy installation of a LAMP or LEMP stack using docker compose

## Environment
**./conf**   
The conf folder holds all the configuration file necessary to install and customize your stack.

**./web**   
The web folder holds the application sources (PHP).

## Installation
From the **./conf/docker** folder copy the **.env** and one of the **docker-compose-xxx** file corresponding to the stack you would like to install.

Mind to rename correctly your file to **docker-compose**

Those files should be place to your **project root**.

## Customize

Most of the configuration can be customize changing environment variables

**.env**   
Holds the global configuration variables

**./conf/container_name/xxx.env**   
Each container configuration (apache/nginx, mysql, and php), could be change by editing the corresponding container_name.env file.

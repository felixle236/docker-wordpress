# docker-wordpress
Docker Wordpress

## Quick Start

- Clone `.env.sample` to `.env` in the same directory and update configuration for project.
- Please make sure MySQL service is running. You can use [docker MySQL](https://github.com/felixle236/docker-mysql).
- Access MySQL and create database if does not exist.
- Start docker container: `docker-compose up` or `docker-compose up -d` (run with background)
- Access to home page with http://localhost
- Refer to docker compose document in [here](https://docs.docker.com/compose/overview/#compose-documentation).

## Start without docker

There are 2 ways to do:
- The first way, export all source code inside docker container is running. Access to docker container and export folder `/var/www/html`.
- The second way, download source code from Wordpress and replace folder `wp-content` from `src/wp-content`, after that copy file `src/.htaccess` to your source (near folder `wp-content`) and update configuration from `.env` to `wp-config.php`.

## Branch prefixes

- bugfix/
- feature/
- hotfix/
- release/

> Exp: feature/feature-name

## Gitflow workflow

<div align="center">
    <img src="https://wac-cdn.atlassian.com/dam/jcr:61ccc620-5249-4338-be66-94d563f2843c/05%20(2).svg?cdnVersion=411" height="400" />
</div>

## CICD pipeline deployment

![CICD pipeline deployment](https://cdn-images-1.medium.com/max/2600/1*1kUhczYDfpkWXSFt0mI2dA.png)

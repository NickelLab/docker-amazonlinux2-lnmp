docker-compose amazonlinux2 lnmp
====

## Description

installed

- docker-compose
- amazonlinux2
- nginx
- mariadb
- php7 (fpm mbstring dom etc...)
- git
- wget
- npm & yarn
- composer

## Usage

### dokcer-compose
```bash
docker-compose up -d
```

### document root for host
```bash
docker-compose.yml/../src/code/public
```

### document root for container
```bash
/srv/public
```

## Author

[NickelLab](https://github.com/NickelLab)
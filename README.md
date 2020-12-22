# TRIPLE ERP DOCKER

## How to run

```bash
$ docker-compose up
```

## How to down

```bash
$ docker-compose down
```

Untuk melihat  list network yang berjalan di docker

```bash
$ docker network ls
```

## How to init Odoo Database
```
1. $ docker-compose exec odoo_docker bash
2. $ odoo -i base -d odoo_db --stop-after-init --db_host=db_postgres -r user_db -w root

```

## How to init Flectra Database
```
1. $ docker-compose exec flectra_docker bash
2. $ flectra -i base -d flectra_db --stop-after-init --db_host=db_postgres -r user_db -w root

```
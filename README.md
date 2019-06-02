# testdriven - microservices
test-drivent.io - microservices

Start docker container in background
```
docker-compose up -d
```
with rebuild image.
```
docker-compose up -d --build
```
Stop docker container.
```
docker-compose down
```
Testing python.
```
docker-compose exec users python manage.py test
```
Recreate database.
```
docker-compose exec users python manage.py recreate_db
```
Attach python shell.
```
docker-compose exec users python manage.py shell
```
Run psql
```
docker-compose exec users-db psql -U postgres
```
Seed data
```
docker-compose exec users python manage.py seed_db
```
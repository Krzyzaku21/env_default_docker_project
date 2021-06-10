## 1. docker django env python3 uwsgi nginx
1. docker-compose up --build
2. docker-compose -f docker-compose.deploy.yml down --volumes
3. docker-compose -f docker-compose.deploy.yml up --build
can use too --build --remove-orphans

## 2. to use python commands
1. docker-compose run --rm app sh -c "python manage.py collectstatic"
2. docker-compose run --rm app sh -c "python manage.py makemigrations"

## 3. to see containsers images docker inside
1. docker ps - to see images IMAGE_ID
2. docker exec -it IMAGE_ID //bin/sh

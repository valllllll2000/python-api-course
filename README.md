# python-api-course

`docker build .`
`docker compose build`
Note: on Linux, we need to use the command `docker compose` instead of `docker-compose`


difference between docker and docker-compose:
https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/Docker-run-vs-docker-compose-Whats-the-difference

create a new django project
`sudo docker compose run --rm app sh -c "django-admin startproject app ."`

create core module
`sudo docker compose run --rm app sh -c "python manage.py startapp core"`

run app service
`docker compose up`

run tests:
`docker compose run --rm app sh -c "python manage.py test"`

clean
`docker compose down`

add `import psycopg2` if psycopg2 errors

Test
`docker compose run --rm app sh -c "python manage.py test"`

Lint
`docker compose run --rm app sh -c "python manage.py wait_for_db"`

Lint
`docker compose run --rm app sh -c "python manage.py wait_for_db && flake8"`
`docker compose run --rm app sh -c "flake8"`




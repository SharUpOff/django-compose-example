# Django Compose Example
This is a sample project demonstrating how to use
[Django](https://www.google.com/search?q=django&oq=django+&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIMCAEQIxgnGIAEGIoFMgYIAhBFGDsyBggDEEUYOzIGCAQQRRg7MgYIBRBFGEEyBggGEEUYPDIGCAcQRRg80gEINDA3MWowajeoAgCwAgA&sourceid=chrome&ie=UTF-8#:~:text=Django%3A%20The%20web,www.djangoproject.com)
with
[Compose](https://docs.docker.com/compose/)
during development.

## Quick start
### Install poetry
```bash
docker compose run example pip install poetry
```

## From scratch
### Init poetry
```bash
docker compose run example poetry init \
  --no-interaction \
  --name example \
  --description 'This is a sample project demonstrating how to use Django with Compose during development' \
  --author 'SharUpOff<sharupoff@efstudios.org>' \
  --license MIT \
  --python 3.12
```
### Add django
```bash
docker compose run example poetry add django~=4.2
```
### Init django
```bash
docker compose run example poetry run django-admin startproject example .
```
### Add django-environ
```bash
docker compose run example poetry add django-environ~=0.11.2
```

## Used services
- https://www.toptal.com/developers/gitignore/api/django

## Used projects
- https://github.com/python-poetry/poetry
- https://github.com/django/django
- https://github.com/joke2k/django-environ

## Used docs
- https://python-poetry.org/docs/configuration/#virtualenvscreate
- https://python-poetry.org/docs/basic-usage/#initialising-a-pre-existing-project
- https://docs.djangoproject.com/en/4.2/intro/tutorial01/#creating-a-project

# OctopusInterface: Brief Documentation

🐙💻

## Setup

### Development

1. Setup .env file
2. `docker-compose build`
3. `docker-compose up db api -d`
4. `cd ./octoinui/`
5. `npm install`
6. `npm run dev`

### Production

Not production ready yet

## Useful Commands

- Freeze the requirements:\
  `pip list --format=freeze > requirements.txt`
- Create a superuser:\
  `docker-compose run --rm api python manage.py createsuperuser`
- Make migrations:\
  `docker-compose run --rm api python manage.py makemigrations`

## Example Data

- Default Test User Password: `1234Password`

## TODO

- Celery Tasks

# OctopusInterface: Brief Documentation

🐙💻

## Vercel & AWS Setup

(Only For non-shady biz Xd)

## GitHub Actions Setup

Currently broke

## Local Setup

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
- Load all fixtures:\
  `docker-compose run --rm api python manage.py load-fixtures`

## Example Data

- Default Test User Password: `1234Password`

## ENVIRONMET VARIABLES

...

## TODO

- Fullfill Order life-cycle
  - Orders Overview
  - Order payout after 2 weeks if no objection (celery needed)
- escrow system
  - payins / payouts for account
  - sloow fees (1.5% suggested)
  - view balance
- messaging
  - between users
- Celery Tasks

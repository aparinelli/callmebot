# callmebot
A bot that sends email reminders.

## How to install

1. Clone the repository:

```
git clone git@github.com:aparinelli/callmebot.git
```

2. Go into the repo directory and create the environment file named `.env`:

```
FLASK_DEBUG=True
DATABASE_URL='postgresql://callmebot:callmebot@db/callmebot'
CELERY_BROKER_URL='redis://redis:6379/0'
CELERY_REDBEAT_REDIS_URL='redis://redis:6379/1'
SECRET_KEY='430c3e5e0aa64fb49ec90aa522c468a2'
MAIL_USERNAME= 'youremail'
MAIL_PASSWORD= 'yourpassword'
```

3. Spin up the docker containers with docker-compose (which you can get by installing Docker Desktop).

```
docker-compose up -d --build
```

4. Go to http://localhost:5010 to use the website!

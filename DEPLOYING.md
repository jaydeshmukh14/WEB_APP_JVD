# Deploying to Heroku

## Prerequisites



```sh
heroku login 

heroku apps 
```

## Server Setup
 a unique name (e.g. "notification-app-123", but yours will need to be different):

```sh
heroku create notification-app-123 
```


```sh
heroku apps
```


```sh
git remote -v
```

## Server Configuration



```sh

heroku config 

heroku config:set APP_ENV="production"

heroku config:set SENDGRID_API_KEY="_________"
heroku config:set SENDER_EMAIL_ADDRESS="someone@gmail.com"

heroku config:set COUNTRY_CODE="US"
heroku config:set ZIP_CODE="20057"
heroku config:set USER_NAME="Jon Snow"
```

```sh
heroku config
```

## Deploying


```sh
git push heroku main
```


## Running the Script in Production


```sh
heroku run bash 

heroku run "python -m app.daily_briefing"
```

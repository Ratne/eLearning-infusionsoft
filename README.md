# Memsion
## Member platform made for Keap Max Classic / Infusionsoft

Memsion is an open source member platform based on Keap max classic user tag where the user can access to a custom membership platform and watch their video resources

Nodejs & Vue3-powered 

## Features

- Webhook from infusionsoft to create an user
- Admin backend to create courses and lessons
- Autologin from infusionsoft email
- Import user from csv

## Env Variables for backend
- PORT: nodejs local port
- URL_PIATTAFORMA: the url of the platform
- BASE_URL: the base url of nodejs
- FRONT_URL=frontend url
- CLIENTID infusionsoft client id
- CLIENTSECRET: infusionsoft client secret
- CALLBACKURL: baseurl+/auth/infusionsoft/callback
- DB_CONNECT: mongodb database
- TOKEN_SECRET= jwt token secret
- EMAIL_HOST= host for email smtp
- EMAIL_USERNAME= smtp email host
- EMAIL_PORT= port smtp host
- EMAIL_PASSWORD= password smtp host
- FROM_EMAIL= from smtp host
- PATH_LOGO= full path logo

## Env Variables for frontend
- VUE_APP_URL= nodejs backend url and port + '/api'
- VUE_APP_APIKEY= tiny.cloud free api key
- VUE_APP_LOGOBRAND= full path to logo


### Sponsor
![Sentry.io](data:image/png;base64,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)
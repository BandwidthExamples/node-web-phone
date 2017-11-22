#node-web-phone

<div> 
<b>This application is outdated, but will be updated soon!</b><br><br>
</div>

NodeJS backend for web-based phone application.

Demos uses of the:
* [Catapult Node SDK](https://github.com/bandwidthcom/node-bandwidth)
* [Creating Application](http://ap.bandwidth.com/docs/rest-api/applications/?utm_medium=social&utm_source=github&utm_campaign=dtolb&utm_content=_)
* [Searching for Phone Number](http://ap.bandwidth.com/docs/rest-api/available-numbers/#resourceGETv1availableNumberslocal/?utm_medium=social&utm_source=github&utm_campaign=dtolb&utm_content=_)
* [Ordering Phone Number](http://ap.bandwidth.com/docs/rest-api/phonenumbers/#resourcePOSTv1usersuserIdphoneNumbers/?utm_medium=social&utm_source=github&utm_campaign=dtolb&utm_content=_)
* [Messaging REST Api Callbacks](http://ap.bandwidth.com/docs/callback-events/text-messages-sms/?utm_medium=social&utm_source=github&utm_campaign=dtolb&utm_content=_)

## Prerequisites
- Configured Machine with Ngrok/Port Forwarding -OR- Heroku Account
  - [Ngrok](https://ngrok.com/)
  - [Heroku](https://www.heroku.com/)
- [Node 4.2+](https://nodejs.org/en/download/releases/)

## Deploy To PaaS

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)


## Install on Local Machine

```bash
# clone the app with submodules

git clone --recursive git@github.com:BandwidthExamples/node-web-phone.git

# install dependencies

npm install

# run the app

cd ..

PORT=3000 npm start 

```

Run in another terminal

```bash
ngrok http 3000 #to make ngrok to open external access to localhost:3000 
```

Open in browser your external url (it will be shown by ngrok).

## Deploy on Heroku Manually

Create account on [Heroku](https://www.heroku.com/) and install [Heroku Toolbel](https://devcenter.heroku.com/articles/getting-started-with-nodejs#set-up) if need.

Run `heroku create` to create new app on Heroku and link it with current project.

Run `git push heroku master` to deploy this project.

Run `heroku open` to see home page of the app in the browser

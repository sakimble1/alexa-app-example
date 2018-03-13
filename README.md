# alexa-js-gm

An test project forked from the alexa-app-example project.  This project uses the [alexa-app](https://github.com/alexa-js/alexa-app) module with Express.  Eventually it will use the ws module to receive websocket connections from a device and forward the alexa requests to the device using a simple json model.
Be warned: I am a noob with node.js and am just pasting together examples from Heroku.

## Deploy
### Deploying locally

Make sure you have [Node.js](http://nodejs.org/) and the [Heroku Toolbelt](https://toolbelt.heroku.com/) installed.

```sh
git clone git@github.com:alexa-js/alexa-app-example.git # or clone your own fork
cd alexa-app-example
npm install
npm start
```

Your app should now be running on **[http://localhost:8080/test](http://localhost:8080/test)**. Put it in your browser to access it's test page.

### Deploying to Heroku

```sh
heroku create
git push heroku master
heroku open
```

Alternatively, you can deploy your own copy of the app using this button:

[![Deploy to Heroku](https://www.herokucdn.com/deploy/button.png)](https://heroku.com/deploy?template=https://github.com/sakimble1/alexa-js-gm)

Your app should now be running on **https://alexa-js-gm.herokuapp.com/test**, where `<app-name>` is the heroku app name. Put it in your browser to access it's test page.

## Changing the endpoint
Depending on where you deployed your app, the path for the endpoint of the skill should have a path parameter at the end called `/test`. If you want to change that, simply change [this](https://github.com/alexa-js/alexa-app-example/blob/master/index.js#L8) line to your desired name.



<img align="center" src="assets/images/backpack.png"></img>

# BackPack: Boilerplate Template for Webpack2 and Heroku

[Webpack 2](https://webpack.js.org/) is super cool, I wrote a sample boiler code that you can reuse to spin a [Express](http://expressjs.com/) application and setup to deploy to [Heroku](https://www.heroku.com/) instantly.

Few things to remember that :

 - **No Fancy** framework or platform are used here, this is clear naked/raw boilerplate, and I'll let you decide to pick your faviorte framework on top of this.

 - This boilerplate use [HMR](https://webpack.js.org/concepts/hot-module-replacement/) and it is cool.

<img align="center" src="assets/images/webpack.gif"></img>

## How to get started ?

Clone this code and follow these instructions

- `npm i`
- `npm start`
- Visit [http://localhost:3000/](http://localhost:3000/)

<img align="center" src="assets/images/npm start.gif"></img>



## Deploy

First, you'll need a heroku account.

- In Heroku, create a new app
- Add a new buildpack, select `heroku/nodejs`. This should set you up to automatically run `npm install` which is what you'll need to get up and running.

<img align="center" src="assets/images/heroku buildpack.gif"></img>


- Follow the instructions to [link to your repository](https://devcenter.heroku.com/articles/git).
- `git push heroku master` - Assuming you've set everything up correctly, this will deploy your app, and run the postinstall script in `package.json`.

## Credits

Thanks to [christianalfoni](https://github.com/christianalfoni) for the excellent [Webpack 1 tutorial and example repo](https://github.com/christianalfoni/webpack-express-boilerplate). I got started there and then built this one once I realized I wanted to play with Webpack v2.

## Notes

The `Heroku` part of this is really easy to change for your own build process. Dig into the npm scripts, and take a look at the production webpack config.

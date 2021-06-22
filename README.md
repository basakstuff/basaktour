<h4 align="center">An awesome tour booking site built on top of <a href="https://nodejs.org/en/" target="_blank">NodeJS</a>.</h4>

 <p align="center">
 <a href="#deployed-version">Demo</a> •
  <a href="#key-features">Key Features</a> •
  <a href="#demonstration">Demonstration</a> •
  <a href="#how-to-use">How To Use</a> •
  <a href="#api-usage">API Usage</a> •
  <a href="#deployment">Deployment</a> •
  <a href="#build-with">Build With</a> •
  <a href="#installation">Installation</a> • 
  <a href="#known-bugs">Known Bugs</a> • 
  <a href="#acknowledgement">Acknowledgement</a>
</p>

## Deployed Version

Live demo (Feel free to visit) 👉 : https://basaktour.herokuapp.com/

## Key Features

- Authentication and Authorization
  - Login and logout
- Tour
  - Manage booking, check tours map, check users' reviews and rating
- User profile
  - Update username, photo, email, and password
- Credit card Payment

## Demonstration

#### Home Page : 
![ScreenRecorderProject66_3](https://user-images.githubusercontent.com/25417307/123008841-4e8f5880-d3c4-11eb-8d36-a905333ccccc.gif)


#### Tour Details : 
![ScreenRecorderProject67](https://user-images.githubusercontent.com/25417307/123008925-7aaad980-d3c4-11eb-83ec-8dac84f980df.gif)


#### Payment Process :
![ScreenRecorderProject68](https://user-images.githubusercontent.com/25417307/123009176-e8570580-d3c4-11eb-9004-05c318d6faf9.gif)


#### Booked Tours :
![Basaktour_My_Tours_-_2021-06-23_01 47 30](https://user-images.githubusercontent.com/25417307/123009232-fefd5c80-d3c4-11eb-81cb-f3471f77c97b.png)



#### User Profile :
![Basaktour_Your_account_-_2021-06-23_01 49 22](https://user-images.githubusercontent.com/25417307/123009380-408e0780-d3c5-11eb-9a29-2f09bbcfe02d.png)


#### Admin Profile :
![Basaktour_Your_account_-_2021-06-23_01 48 15](https://user-images.githubusercontent.com/25417307/123009291-1b00fe00-d3c5-11eb-83ff-608e9ee250b6.png)

## How To Use

### Book a tour

- Login to the site
- Search for tours that you want to book
- Book a tour
- Proceed to the payment checkout page
- Enter the card details (Test Mood):
  ```
  - Card No. : 4242 4242 4242 4242
  - Expiry date: 02 / 22
  - CVV: 222
  ```
- Finished!

### Manage your booking

- Check the tour you have booked in "Manage Booking" page in your user settings. You'll be automatically redirected to this
  page after you have completed the booking.

### Update your profile

- You can update your own username, profile photo, email and password.

## API Usage

Before using the API, you need to set the variables in Postman depending on your environment (development or production). Simply add:

```
- {{URL}} with your hostname as value (Eg. http://127.0.0.1:3000 or http://www.example.com)
- {{password}} with your user password as value.
```

Check [Basaktour API Documentation](https://documenter.getpostman.com/view/9241484/TzeTJpTF) for more info.

<b> API Features: </b>

Tours List 👉 https://127.0.0.1:3000/api/v1/tours

Tours State 👉 https://127.0.0.1:3000/api/v1/tours/tour-stats

Get Top 5 Cheap Tours 👉 https://127.0.0.1:3000/api/v1/tours/top-5-cheap

Get Tours Within Radius 👉 https://127.0.0.1:3000/api/v1/tours/tours-within/200/center/34.098453,-118.096327/unit/mi

## Deployment

The website is deployed with git into heroku. Below are the steps taken:

```
git init
git add -A
git commit -m "Commit message"
heroku login
heroku create
heroku config:set CONFIG_KEY=CONFIG_VALUE
parcel build ./public/js/index.js --out-dir ./public/js --out-file bundle.js
git push heroku master
heroku open
```

You can also changed your website url by running this command:

```
heroku apps:rename basaktour-users
```

## Build With

- [NodeJS](https://nodejs.org/en/) - JS runtime environment
- [Express](http://expressjs.com/) - The web framework used
- [Mongoose](https://mongoosejs.com/) - Object Data Modelling (ODM) library
- [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) - Cloud database service
- [Pug](https://pugjs.org/api/getting-started.html) - High performance template engine
- [JSON Web Token](https://jwt.io/) - Security token
- [ParcelJS](https://parceljs.org/) - Blazing fast, zero configuration web application bundler
- [Stripe](https://stripe.com/) - Online payment API
- [Postman](https://www.getpostman.com/) - API testing
- [Mailtrap](https://mailtrap.io/) & [Sendgrid](https://sendgrid.com/) - Email delivery platform
- [Heroku](https://www.heroku.com/) - Cloud platform

## Installation

You can fork the app or you can git-clone the app into your local machine. Once done that, please install all the
dependencies by running

```
$ npm i
set your env variables
$ npm run watch:js
$ npm run build:js
$ npm run dev (for development)
$ npm run start:prod (for production)
$ npm run debug (for debug)
$ npm start
Setting up ESLint and Prettier in VS Code 👇
$ npm i eslint prettier eslint-config-prettier eslint-plugin-prettier eslint-config-airbnb eslint-plugin-node
eslint-plugin-import eslint-plugin-jsx-a11y  eslint-plugin-react --save-dev
```

## Known Bugs

Feel free to email me at basaker98@gmail.com if you run into any issues or have questions, ideas or concerns.
Please enjoy and feel free to share your opinion, constructive criticism, or comments about my work. Thank you! 🙂

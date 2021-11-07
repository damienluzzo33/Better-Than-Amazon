# Better-Than-Amazon - An E-Commerce Backend App

## Description

In the world of E-Commerce, everyone is chasing Amazon... But what if there was something better than Amazon? Well, while there may be something one day that is, this app comes nothing close to Amazon. In fact, this is a purely backend routing and CRUD implementation exercise. 

However, if you instead are looking for a purely backend operation to organize your retail business assets, then this is the app for you! Feel free to create, view, update or delete anything and everything relating to products, product categories, and product tag information.

Feel free to test all the routes and do your best to break it! Improvements are always needed! If you are interested in improving or modifying this application for your own personal usage, please go ahead and clone down the repository and transform it into your own amazing E-Commerce Backend App.

[Link to video demo of app](https://drive.google.com/file/d/1c5WZS1QpqnIaY9XuwP1zGG6J_n3uwsxm/view)

![Giphy demo of project](./images/bta_gif.gif)

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Credits](#credits)
- [License](#license)
- [Features](#features)
- [Examples/Tests](#examples)

## Installation

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

- To install the app, simply clone down this repository to your local machine

## Usage

- To use the application, just navigate to the cloned down repository, and run "npm i" to get the necessary node modules

- Next, you will need to open up the MySQL server on the root level of the repository using "mysql -u your_username -p" and then enter your mysql password

- Once logged into MySQL through the terminal you need to run the schema using "SOURCE db/schema.sql" then run "quit" to exit mysql

- Once you exit mysql, run the seeds using "npm run seed"

- You'll then want to get the server started by running "npm run watch"

- Finally, launch something like Insomnia or Postman and hit the routes!

## Credits

Assets:

+ [express by express](https://expressjs.com/)

+ [sequelize by sequelize](https://github.com/sequelize/sequelize)

+ [mysql2 by sidorares](https://github.com/sidorares/node-mysql2)

## License

+ MIT

## Features

+ User is able to create, view, update, and delete products and product categories using Insomnia or Postman

+ Data from user submissions updates the connected MySQL database

## How to Contribute

If you would like to contribute to the Better-Than-Amazon E-Commerce App, please feel free to clone or fork this repository and implement your desired improvements. Once your improvements have been made and the app has been tested properly, please feel free to send me a message on github with a short summary of the changes you've made and I will invite you to be a collaborator.

## Examples

### CREATE PRODUCT
---

Send your post and put requests to "/api/products/" and "/api/products/:id" respectively

+ Your JSON post requests should have the form: 
```
{
	"product_name": "Basketball",
	"price": 20.00,
	"stock": 3,
	"tagIds": [1, 2, 3, 4],
	"category_id": 2
}
```
+ Your JSON put requests should have the form: 
```
{
	"product_name": "Football",
	"price": 15.00,
	"stock": 6,
	"tagIds": [1, 2, 3, 4],
	"category_id": 2
}
```

### CREATE / UPDATE CATEGORY
---

Send your post and put requests to "/api/categories" and "/api/categories/:id" respectively

+ Your JSON post request should have the form: 
```
{
	"category_name": "Belts"
}
```
+ Your JSON put request should have the form: 
```
{
	"category_name": "Sandals"
}
```

### CREATE / UPDATE TAG
---

Send your post and put requests to "/api/tags" and "/api/tags/:id" respectively

+ Your JSON post request should have the form: 
```
{
	"tag_name": "chuck"
}
```
+ Your JSON put request should have the form: 
```
{
	"tag_name": "jack"
}
```
To see more examples for how to use the app and what kind of json data is needed, please refer to the video in the description above.

## Questions

Connect with me on GitHub: [damienluzzo33](https://www.github.com/damienluzzo33)

Shoot me an email: [damienluzzo33@gmail.com](mailto:damienluzzo33@gmail.com)

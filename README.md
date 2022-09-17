# E-Commerce

## Table of contents

- [Overview](#overview)
 - [The challenge](#the-challenge)
  - [User Story](#user-story)
  - [Acceptance Criteria](#acceptance-criteria)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)


## Overview

### The challenge
The challenge is to build the back end for an e-commerce site by configuring an Express.js API to use Sequelize to interact with a MySQL database.


### User Story

AS A manager at an internet retail company
I WANT a back end for my e-commerce website that uses the latest technologies
SO THAT my company can compete with other e-commerce companies

### Acceptance Criteria

GIVEN a functional Express.js API
WHEN I add my database name, MySQL username, and MySQL password to an environment variable file
THEN I am able to connect to a database using Sequelize
WHEN I enter schema and seed commands
THEN a development database is created and is seeded with test data
WHEN I enter the command to invoke the application
THEN my server is started and the Sequelize models are synced to the MySQL database
WHEN I open API GET routes in Insomnia Core for categories, products, or tags
THEN the data for each of these routes is displayed in a formatted JSON
WHEN I test API POST, PUT, and DELETE routes in Insomnia Core
THEN I am able to successfully create, update, and delete data in my database

### Screenshot

![](./assets/images/screenshot1.png)
![](./assets/images/screenshot2.png)

### Links

- Solution URL: [E-Commerce](https://github.com/Monkonjay/E-Commerce)

- Video Demo: [GET Routes for all Categories, Products, Tags](https://drive.google.com/file/d/18xV6HPOcLHu_XxONpWlBqhptsFph5DFR/view)

- Video Demo: [GET Routes for a single Category, Product, Tag](https://drive.google.com/file/d/1U-vTZ8Kn6oTQMtnTa2ksLBE8v1gmFjec/view)

- Video Demo: [POST, PUT, DELETE for Categories](https://drive.google.com/file/d/1-boVV80x9Gr4GXprQKR8nLv-UXCi02UQ/view)

- Video Demo: [POST, PUT, DELETE for Products](https://drive.google.com/file/d/1mfbO7p_MkO04xQ58U0E-iKIgOjYDivZj/view)

- Video Demo: [POST, PUT, DELETE for Tags](https://drive.google.com/file/d/15XJ1hMjDyP_Pd0RhUao50SSzV9II3F9A/view)

## My process

### Built with

- Express.js
- Sequelize
- MySql


### What I learned

During this project, I used Sequelize to interact with the MySQL database to perform CRUD operations and used Express routes to navigate the app. 


```Javascript Express.js, Sequelize
  router.post('/', (req, res) => {
  // create a new category
  const newCategory = req.body;
  Category.create(newCategory)
.then (categories => res.json(categories)) 
.catch(err => res.status(500).json(err));

});
```


## Author

- Website - [Robert M Greene]( https://monkonjay.github.io/Portfolio/)
- Github - [Monkonjay](https://github.com/Monkonjay)
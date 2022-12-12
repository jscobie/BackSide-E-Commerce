# Challenge 13 ORM: E-Commerce Back End

## Badges
[![License: CC0-1.0](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Description

This goal of this challenge is to build the back end for an e-commerce site. Due to the prevalence of these e-commerce platforms, developers should understand the fundamental architecture of e-commerce sites. I was tasked with starting with a working Express.js API and configure it to use Sequelize to interact with a MySQL database. I needed to edit the following files to add related data based on the challenge requirements:
* Files under ***models*** folder:
    * Category.js, Product.js, ProductTag.js, and Tag.js - needed columns defined for each table/model
    * index.js - needed relationships of tables added
* Files in the ***root (/)*** folder:
    * server.js in / folder - needed to import sequelize connection added and sync'ing of models before starting the server
* Files under ***routes*** folder:
    * product-routes.js, tag-routes.js, and category-routes.js - needed complete route builds for various get, post, put/patch, and delete

### Required links for review and grading submission
[Github Repository Link](https://github.com/jscobie/BackSide-E-Commerce)<br>
[Video walkthrough of completed database build and populate. application start, and Insomia results](https://drive.google.com/file/d/1R2KS5Abt-DcnDB5KVsCNizCa_3IhBfM-/view)

## Table of Contents

* [Description](#description)
* [Installation](#installation)
* [Usage](#usage)
* [License](#license)
* [Tests](#tests)
* [Credits](#credits)
* [Questions?](#questions)

## Installation

**1. Clone to your computer using SSH from GitHub:**
```
git clone git@github.com:jscobie/BackSide-E-Commerce.git
```
**2. You'll need to run to install the node required dependencies after you clone the install by running:**
```
npm install
```
**3. You will need to make an .env file to handle the MySQL connection, an example file (.env.EXAMPLE) has been included for you to reference. Contents of .env.EXAMPLE are:**
```
DB_USER=''
DB_PASSWORD=''
DB_DBASE='employee_db'
```
**4. You will then need to run the following commands in your MySQL server command line to build the database and tables and then seed/populate the tables needed:**
```
- mysql -u root -p
- <enter password>
- SOURCE db/schema.sql
- USE ecommerce_db;
```
**5. You will need to seed the database:**
```
node /seeds/index.js
```
**6. Finally to start the Employee Tracker you need the command:**
```
npm start
```

## Usage

The usage of this project is to allow myself to turn this project in for grading to the MSU Bootcamp academic grading team.

## License
Read more about [MIT license](https://opensource.org/licenses/MIT).

## Tests

The tests to confirm working are all performed in Insomnia, included in the walkthrough video and explained below:
***Tags*** tests:
| HTTP Request Type | URL example                        | Output                        |
| ----------------- | ---------------------------------- | ----------------------------- |
| GET               | localhost:3001/api/tags            | View all data                 |
| GET               | localhost:3001/api/tags/3          | View data for specified id    |
| POST              | localhost:3000/api/tags            | Add new data                  |
| PUT               | localhost:3000/api/tags/3          | Update data for specificed id |
| DELETE            | localhost:3000/api/tags/3          | Delete data for specified id  |

***Categories*** tests:
| HTTP Request Type | URL example                        | Output                        |
| ----------------- | ---------------------------------- | ----------------------------- |
| GET               | localhost:3001/api/categories      | View all data                 |
| GET               | localhost:3001/api/categories/3    | View data for specified id    |
| POST              | localhost:3000/api/categories      | Add new data                  |
| PUT               | localhost:3000/api/categories/3    | Update data for specificed id |
| DELETE            | localhost:3000/api/categories/3    | Delete data for specified id  |

***Products*** tests:
| HTTP Request Type | URL example                        | Output                        |
| ----------------- | ---------------------------------- | ----------------------------- |
| GET               | localhost:3001/api/products        | View all data                 |
| GET               | localhost:3001/api/products/3      | View data for specified id    |
| POST              | localhost:3000/api/products        | Add new data                  |
| PUT               | localhost:3000/api/products/3      | Update data for specificed id |
| DELETE            | localhost:3000/api/products/3      | Delete data for specified id  |

## Credits

Credit to the MSU Bootcamp and instructors for training and training materials to resolve some of these issues.<br>
*Programs, packages used:*<br>
[Node.js](https://nodejs.org/en/)<br>
[Insomnia (for testing)](https://insomnia.rest/)<br>
[Sequelize](https://sequelize.org/)<br>
[Express JS](https://expressjs.com/)<br>
[Mysql2 npm package](https://www.npmjs.com/package/mysql2)<br>
[dotenv npm package](https://www.npmjs.com/package/dotenv)

## Questions:
*Use the following options to contact me for questions:*<br>
[jscobie](https://github.com/jscobie)<br>
jscobie@focus-solutions.net
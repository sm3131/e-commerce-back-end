# E-Commerce Back End

[![License Badge](https://img.shields.io/badge/license-MIT-green)](https://opensource.org/licenses/MIT)

## Description

This project contains the back end code for an e commerce application. The code for this project provides the server side functionality, as well as the api routes, and database files. With this code a front end could be created to develop a fully functional e commerce application. This project allows the user to create the starter database with some initial seed data, and then before creating a front end they could test all of the GET, POST, PUT, and DELETE routes in an app such as Insomnia to see how these routes function. 

## Table of Contents
  * [Built With](#built-with)
  * [Code Access](#code-access)
  * [Preview](#preview)
  * [Installation](#installation)
  * [Usage](#usage)
  * [License](#license)
  * [Questions](#questions)
  * [Credits](#credits)

## Built With

The E-Commerce Back End application was built with:
- JavaScript
- Node.js
- File System
- npm
- Sequelize
- mySQL
- Express.js

## Code Access

If you would like to access the code for this back-end application, please visit [GitHub](https://github.com/sm3131/e-commerce-back-end)

## Preview

Click on the links below to watch the Screencastify videos that demonstrate the e-commerce back-end to the user.

Part 1:
https://watch.screencastify.com/v/aAuaoyX2oiPVRa54UYGw

Part 2:
https://watch.screencastify.com/v/9Y5oHYFDGbKJqIK3aHhG

Part 3:
https://watch.screencastify.com/v/FMacF6b97g0cCfF4reae

View the videos above to see how the routes display various JSON responses to each request. All of the GET, POST, PUT, and DELETE routes are shown in the videos above. 

## Installation
To install the E-Commerce back-end application complete the following steps:
1. Clone the application's code from this [GitHub](https://github.com/sm3131/e-commerce-back-end) repository onto your local machine into a new directory (e.g. e-commerce-back-end).
2. Open the command line and navigate to the directory you cloned this repository into, then open the content in a code text editor. You should now see the main files and folders for this project (server.js, package.json, /seeds, /routes, /models).
3. Next check to see if you have node.js installed on your machine by running the command *node -v* in your command line.
4. If you have node.js make sure your version is up to date by going to this website (https://nodejs.org/en/).
5. If you do not have node.js installed follow the installation steps on this website (https://nodejs.org/en/).
6. Once you have node.js installed, make sure you are still in the e-commerce directory in the command line, and then run the following command *npm install* to install the required packages and dependencies to run the application.
7. Next you will need to make sure you have mysql installed in the command line to create the e-commerce_db database for this application in the mysql shell. Follow this link (https://dev.mysql.com/doc/mysql-installation-excerpt/5.7/en/) to install and run mysql on your local machine. In this project's directory in the mysql shell run the command *source db/schema.sql* to add the database to mysql.
8. Next you will need to download an application called Insomnia to test all of the routes this back-end application provides. To install Insomnia follow the steps on this site (https://docs.insomnia.rest/insomnia/get-started).
9. After you have node.js, mysql, Insomnia, and the required npm dependencies installed, you are ready to start the express server via node.js using the command line, in order to test the routes in Insomnia.

## Usage
To use and test the e-commerce routes in Insomnia complete the following steps:
1. The purpose of this application is to create a properly functioning back-end that could be used in conjunction with an e-commerce front-end to create a fully functional website. 
2. After you have completed all of the above installation steps, make sure you seed the data tables by running *npm run seed*, then you can now start your express server and test the routes in Insomnia.
3. To start the server using the command line, type *npm start* and you should see a notification stating "App listening on port 3001!", meaning your server is functioning properly.
4. If the server is running properly you can now head over to the Insomnia application you downloaded in the installation steps and set up a request collection to start organizing your route requests.
5. Once in Insomnia you will have an option to create a new request collection, which you can title e-commerce for example, then within this collection you can create a folder for each collection of the routes in this application (i.e. category-requests, product-requests, tag-requests), or if you prefer you can just put them all on the same screen.
6. Once you have created your route folders, you can start making a file for each individual request in each folder which would be the GET, POST, PUT, and DELETE requests.
7. Now in each individual request file you will need to either enter just the endpoint in the top URL bar for GET and DELETE requests, or you will need to enter the endpoint and a JSON formatted body for POST and PUT requests.
8. If you are running this app locally, then according to your server you will be on port 3001, so the correct endpoint for every route will start with localhost:3001/api, then the end portion of the endpoint will vary depending on the request and which specific route your are trying to test.
9. So an example GET request to get all the products would be formatted as: localhost:3001/api/products then the dropdown request bar should be GET.
10. Again check to make sure your server is running in the command line, and then you can hit send on the request to GET all of the current products in the database. 
11. If you need to know which endpoints to use for each of the routes you can refer to the routes folder in your code editor, and see that they all start with localhost:3001/api, then the final endpoint will either contain categories, products, or tags and then possibly an ID number if you are doing a GET by Id route, PUT route, or DELETE route

**IMPORTANT NOTE:** Ensure that your server is running properly before testing routes, and make sure that you have entered the correct endpoints to properly execute your requests. 

## License

MIT License

Copyright (c) 2022 Sammi Moore

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Questions

If you would like to access this project's repository as well as other projects in my GitHub, click this [GitHub](https://github.com/sm3131) link. 

For all other questions or inquires please feel free to contact me via email at [sm2683@nau.edu](mailto:sm2683@nau.edu)

## Credits

The initial starter code for this project was provided by [Xandromus](https://github.com/coding-boot-camp/fantastic-umbrella), this code contained the seeds data, some of the routes, and boilerplate code for the index.js and server.js files. All of the models and almost every route was created by myself, Sammi Moore.

The resources that I used for this project are as follows:
- The sequelize package from npm in this node.js application in order more easily use mysql databases (https://www.npmjs.com/package/sequelize)
- The mysql2 package from npm to create and store the database and data (https://www.npmjs.com/package/mysql2)
- The express package from npm to create the server and routes (https://www.npmjs.com/package/express)
- The dotenv package from npm to to hide mysql passwords and usernames when pushing code to GitHub (https://www.npmjs.com/package/dotenv)
- https://opensource.org/licenses/ (To borrow the license section text describing the terms of each of the licenses included in the readme generator)
- https://shields.io/ (To generate the link to create the license badge)
For the license badges and license section of the readme, I used the following resources:
- https://choosealicense.com/ (To help with picking which licenses to include)
- https://shields.io/ (To generate the link to create the license badge)
- https://wisehackermonkey.github.io/badge-demo/ (To help with coloring the license badges and grabbing the license links)
- https://opensource.org/licenses/ (To borrow the license section text describing the terms of the licenses included in the readme)

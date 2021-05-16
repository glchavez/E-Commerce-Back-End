# E-Commerce-Back-End

An e-commerce site backend that provides store owners the ability to update products, product tags, and categories in their store database.

## Overview

This application represents the back end of an e-commerce site. A working Express.js API was configured to use Sequelize to interact with a MySQL database holding seeded store item data. Within the application, you're able to run various CRUD operations with the database. It is intended to create quick and easy interactions with an e-commerce database for the owner and their clients.

A challenge I faced when creating this repository was writing the mySQL queries and connecting data between tables in the database. For future improvements, I would like to create the front-end of this application to create a basic, functional e-commerce store.

## Installation

To install this repository for use, you will need to download all files in the [E-Commerce-Back-End](https://github.com/glchavez/E-Commerce-Back-End) repository. You will also need to connect sequelize to use your own local database and credentials within the connection.js file located in the config folder.

Please note, you will need node.js to run this repository on your computer.

## Usage

You will first need to open the connection.js file within the config folder and connect your local database for usage. Do not forget to create a .env file that holds your personal information.

To create the database with starting sample data, run the "npm run seed" command within your integrated terminal of VS Code. Then run the "npm run start" command to connect the server with the database. Once this is done, open Insomnia Core to run the localhost url's and perform CRUD operations (More information on each CRUD operation can be found within the routes folder).

Below is a sample list of the different URL's that can be used. Please note you can change the ending numbers of these URL's to reference different items in the database by id number.

Tag-Routes:

<ul>
<li>Get all tags: http://localhost:3001/api/tags/</li>
<li>Get a tag by id: http://localhost:3001/api/tags/4</li>
<li>Post a tag: http://localhost:3001/api/tags/</li>
<li>Put a tag: http://localhost:3001/api/tags/9</li>
<li>Delete a tag: http://localhost:3001/api/tags/9</li>
</ul>

Product-Routes:

<ul>
<li>Get all products: http://localhost:3001/api/products/</li>
<li>Get a product by id: http://localhost:3001/api/products/3</li>
<li>Post a product: http://localhost:3001/api/products/</li>
<li>Put a product: http://localhost:3001/api/products/6</li>
<li>Delete a product: http://localhost:3001/api/products/6</li>
</ul>

Category-Routes:

<ul>
<li>Get all categories: http://localhost:3001/api/categories/</li>
<li>Get a tag category id: http://localhost:3001/api/categories/3</li>
<li>Post a category: http://localhost:3001/api/categories/</li>
<li>Put a category: http://localhost:3001/api/categories/6</li>
<li>Delete a category: http://localhost:3001/api/categories/6</li>
</ul>

For a video example, please click this [link](https://drive.google.com/file/d/1INRPNXXYIX7hB6WYs4N61YRQ8HAeiBIw/view?usp=sharing).

## Credits

I would like to provide credit to [The Denver Univeristy Coding Bootcamp](https://bootcamp.du.edu/coding/) for providing me with the materials, intstructions, and one-on-one assistance to perform this project.

## License

MIT License

Copyright &copy; 2021 Giovany Chavez

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

# eCommerce Back End

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Description

I was motivated to create the back end processes for an eCommerce business. This project sets up a database and seeds and allows a user to enter in additional categories, products, and tags. 

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [Questions and Contributing](#questions-and-contributing)
- [Tests](#tests)

## Installation

1) Clone this repository onto your computer and ensure you have all of the necessary programs (Git Bash, Node.js, SQL, and Insomnia installed).
2) Run "npm i" in the terminal to install the rest of the necessary tools for this project to work.
3) Add a ".env" file with the database, username, and password filled out as follows:

            DB_NAME='ecommerce_db'
            DB_USER='ENTER USERNAME HERE'
            DB_PASSWORD='ENTER PASSWORD HERE'

4) Log into mysql and source the schema.sql.

            First command: mysql -u root -p
            Second command: source db/schema.sql;

5) Run the seeds.

            Command: npm run seed

6) Run "npm start" in the terminal.

7) Pull up the project in Insomnia using http://localhost:3001/. The application is now ready for use.

## Usage

When the user runs a GET request in Insomnia, using either the api/categories path, the api/products path or the api/tags path, the user will then be presented with a list of all of the respective categories, products, or tags. This will look something like the following:

    http://localhost:3001/api/categories

The user can then run a GET request with the previous path plus "/" and the "id" (for example: categories/1) and they will get a response with just the information for the id of 1. This will look something like the following:

    http://localhost:3001/api/categories/1

The user can then run a POST request with the body filled out with the first mentioned path and the the application will add either a category, a product, or a tag. This will look something like the following:

    http://localhost:3001/api/categories

If the user runs a PUT request with the second mentioned path, they will be able to change the category, product, or tag connected with the id entered. This will look something like the following:

    http://localhost:3001/api/categories/1

Finally, the user can run a DELETE request with the second mentioned path and the category, product, or tag connected with the id entered will be removed. This will look something like the following:

    http://localhost:3001/api/categories/1

### Examples of use:

Categories:

[![Video of program use, providing a visual of options and usage when running the program in the terminal.](./Images/Categories.gif)](https://drive.google.com/file/d/1eOY49th4S-_Kzn6ObgD9aTHNeiE5Yf6V/view)

Products:

[![Video of program use, providing a visual of options and usage when running the program in the terminal.](./Images/Products.gif)](https://drive.google.com/file/d/1SOHWnC89wqzMO36f5lkh_Ue3ihzmVB97/view)

Tags:

[![Video of program use, providing a visual of options and usage when running the program in the terminal.](./Images/Tags.gif)](https://drive.google.com/file/d/1pTDY_90P6az0CBrDhy3egc1tfZQ4J7xC/view)


## License

[The MIT License](https://opensource.org/licenses/MIT)

## Questions and Contributing

If you have any questions, you can contact me by [email](j.mcd.lungren@gmail.com) or through [GitHub](https://github.com/jmcdlungren).

If you are interested in contributing, please follow the guidelines outlined within the [Contributor Covenant](https://www.contributor-covenant.org/).

## Tests

N/A
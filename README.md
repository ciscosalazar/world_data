# World Data

This is a personal data analysis project using **MySQL** and **Python**. The goal of the project is to practice and strengthen my skills in data analysis, working with databases, and Python programming.

## Table of Contents

- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Usage](#usage)
- [Results](#results)
- [Data Import](#data-import)
- [License](#license)
- [FAQ](#faq)

## Installation

To set up this project locally, follow these steps:

1. Clone this repository:

```bash
git clone https://github.com/your-username/word-data.git
```

2. Install the required dependencies:

```bash
pip install -r requirements.txt
```

3. Ensure you have Python 3.10.13 or higher installed.

4. Install Jupyter notebook

```bash
pip install notebook
```

## Environment Variables

To run this project, you need to configure the following environment variables. Create a `.env` file in the root directory of the project and add the variables below:

```
DB_DIALECT=mysql
DB_USERNAME=your_username
DB_PASSWORD=your_password
DB_HOST=localhost
DB_DATABASE=your_database
```

Make sure to replace the placeholders with your actual database credentials.

## Usage

Once the dependencies are installed and the environment variables are set up, launch Jupyter Notebook with the following command:

```bash
jupyter notebook
```

This will open Jupyter Notebook in your browser. Open the notebook file and run the cell to initiate the data analysis process using the configuration from your `.env` file.

## Results

To visualize the population data on a map, click the image below to view the map:

[![Population Map](https://ciscosalazar.github.io/world_data/map_with_population_info_eu_thumbnail.png)](https://ciscosalazar.github.io/world_data/map_with_population_info_eu.html)

## Data Import

The SQL files used to populate the database can be found in the `/sql` directory. These queries include all the necessary operations to set up the database.

For example:

```sql
-- sql/create_table_country.sql
CREATE TABLE country (
    id INT PRIMARY KEY,
    name VARCHAR(255),
    population INT
);
```

The SQL scripts are provided for setting up the database structure and importing the data.

## License

This project is licensed under the **Proprietary License**. You may not use, distribute, or modify this project without my explicit permission. Please contact me if you wish to inquire about usage rights.

## FAQ

#### Question 1: How do I set up the MySQL database for this project?

Answer: You need to create a MySQL database and configure the connection in the `.env` file as described in the [Environment Variables](#environment-variables) section.

#### Question 2: What Python version is required to run this project?

Answer: This project requires Python 3.10.13 or later.

#### Question 3: How do I install the required dependencies?

Answer: Follow the installation instructions provided in the [Installation](#installation) section to install the necessary dependencies using pip.

#### Question 4: How can I run the SQL queries provided?

Answer: The SQL queries are located in the `/sql` directory. You can run these queries directly in your MySQL database using a MySQL client or command line interface. Make sure to adjust the database connection settings in the `.env` file before running the queries.

#### Question 5: What should I do if the database connection fails?

Answer: Ensure that your `.env` file contains the correct database credentials. If you encounter connection issues, check your MySQL server's status and ensure that it is running. Additionally, make sure that firewall settings are not blocking the connection to the database.

#### Question 6: Can I use this project with a database other than MySQL?

Answer: Currently, this project is configured to work with MySQL. However, you can modify the database connection settings in the code to work with other relational databases such as PostgreSQL or SQLite.

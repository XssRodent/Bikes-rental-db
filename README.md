# Build a Bike Rental Shop

This project is part of the FreeCodeCamp curriculum, where you will create an interactive Bash program that simulates a bike rental shop. The program will store rental information in a PostgreSQL database, allowing users to rent bikes and manage rentals.

## Table of Contents

- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Project Setup](#project-setup)
- [Features](#features)
- [Usage](#usage)
- [Database Structure](#database-structure)
- [Project Requirements](#project-requirements)
- [License](#license)

## Project Overview

In this 210-lesson course, you will develop a command-line application to manage a bike rental shop. The application will interact with a PostgreSQL database to handle customer and rental data. You'll gain hands-on experience with Bash scripting and PostgreSQL, building skills in database management, data retrieval, and scripting automation.

## Technologies Used

- **Bash Scripting**: To create an interactive command-line program.
- **PostgreSQL**: To store and manage data related to the bike rental shop.
- **psql**: PostgreSQL command-line interface for database interaction.

## Project Setup

To get started with the project, follow these steps:

1. **Install PostgreSQL**: Ensure you have PostgreSQL installed on your system. You can download and install it from the [official PostgreSQL website](https://www.postgresql.org/download/).

2. **Clone the Repository**: Clone this repository to your local machine using:
    ```bash
    git clone https://github.com/yourusername/bike-rental-shop.git
    cd bike-rental-shop
    ```

3. **Create the Database**: Log in to the PostgreSQL prompt and create the necessary database for the project:
    ```bash
    psql --username=postgres
    CREATE DATABASE bikeshop;
    ```

4. **Set Up the Tables**: Run the provided SQL script to create the required tables and schema:
    ```bash
    psql -U postgres -d bikeshop -f setup.sql
    ```

5. **Run the Bash Script**: Execute the main script to start the bike rental shop program:
    ```bash
    ./rental_shop.sh
    ```

## Features

- **Add New Bikes**: Add information about new bikes to the inventory.
- **Rent a Bike**: Rent out bikes to customers and store rental details.
- **Return a Bike**: Process bike returns and update rental information.
- **View Inventory**: Display available bikes for rent.
- **Customer Management**: Store and manage customer information.

## Usage

1. **Launch the Program**: Run the `rental_shop.sh` script to start the program.

2. **Main Menu**: The program will display a main menu with options such as renting a bike, returning a bike, viewing the inventory, and managing customer information.

3. **Input Commands**: Use the command-line interface to navigate through the options and interact with the bike rental shop system.

4. **Exit**: You can exit the program at any time by selecting the exit option from the menu.

## Database Structure

The PostgreSQL database for the bike rental shop consists of the following tables:

1. **bikes**: Stores information about each bike, including bike ID, model, brand, and availability status.

2. **customers**: Stores customer details such as customer ID, name, phone number, and email.

3. **rentals**: Records rental transactions, including rental ID, bike ID, customer ID, rental date, return date, and rental status.

## Project Requirements

- You must have PostgreSQL installed on your local machine.
- Basic knowledge of SQL and Bash scripting is required.
- Follow the lessons in sequence to build and expand the project functionality step-by-step.

## License

This project is part of the FreeCodeCamp curriculum and is licensed under the [MIT License](LICENSE).

## Acknowledgments

- Thanks to [FreeCodeCamp](https://www.freecodecamp.org/) for providing this course and its comprehensive curriculum.

# Budget Manager Web Application

![Budget Manager](link-to-your-splash-screen-image)

This is a Ruby on Rails application that allows you to manage your budget by tracking your transactions and categorizing your expenses. With Budget Manager, you can easily monitor your spending habits and gain insights into where your money goes.

## Table of Contents

- [Design](#design)
- [Interactions](#interactions)
  - [Splash Screen](#splash-screen)
  - [Sign Up and Log In Pages](#sign-up-and-log-in-pages)
  - [Home Page (Categories Page)](#home-page-categories-page)
  - [Transactions Page](#transactions-page)
  - [Add a New Category Page](#add-a-new-category-page)
  - [Add a New Transaction Page](#add-a-new-transaction-page)
- [Testing](#testing)
- [Technical Requirements](#technical-requirements)
- [Database Schema](#database-schema)

## Design

The design of the Budget Manager application is based on the guidelines provided by Gregoire Vella on Behance. The Creative Commons license requires us to give appropriate credit to the author. Please make sure to include the following credit in your project's README:

"Design inspired by Gregoire Vella's work on Behance. [Link to the original design](link-to-the-design)."

To maintain consistency and a visually pleasing interface, follow the design guidelines in terms of colors, typography (font face, size, and weight), and layout composition. Note that some UI elements shown in the design guidelines may not be applicable to this exercise, and you will need to create additional pages based on the existing design guidelines.

## Interactions

### Splash Screen

Upon accessing the application, users will be greeted with a simple splash screen that displays the name of the app and provides links to the sign-up and log-in pages.

### Sign Up and Log In Pages

Users can register for an account by providing their full name, email address, and password (all mandatory fields). Once registered, users can log in using their email and password. Access to pages that require authentication will be restricted to logged-in users only.

### Home Page (Categories Page)

After logging in, users will be directed to the categories page, which serves as the home page. On this page, users can view a list of categories along with their respective icons and the total amount of money spent in each category. Clicking or tapping on a category item will navigate the user to the transactions page for that category. At the bottom of the page, there is a button to add a new category, which leads to the "Add a New Category" page.

### Transactions Page

The transactions page displays a list of transactions for a selected category, sorted by the most recent entries. The page also shows the total amount spent within the category, calculated as the sum of all transaction amounts. At the bottom of the page, there is a button to add a new transaction, redirecting the user to the "Add a New Transaction" page. Clicking the "Back" button (<) will navigate the user back to the home page.

### Add a New Category Page

On this page, users can fill out a form to create a new category. The form requires the user to enter a category name and select an icon for the category (both fields are mandatory). Clicking the "Save" button will save the new category and redirect the user to the home page. The "Back" button (<) returns the user to the home page.

### Add a New Transaction Page

Users can add a new transaction by completing a form with the following details:
- Name (mandatory)
- Amount (mandatory)
- Categories (mandatory, at least one)

After filling out the form, users

 can click the "Save" button to create the new transaction. Upon successful creation, the user will be redirected to the transactions page for the respective category. The "Back" button (<) allows the user to return to the transactions page for that category.

## Testing

To ensure the reliability and functionality of your Ruby on Rails application, it is essential to create unit and integration tests for all the critical components. Implement comprehensive testing to cover various scenarios and validate the correctness of your application's behavior.

## Technical Requirements

To meet the project's specifications, the following technical requirements must be fulfilled:

- Use Postgres as your database.
- Utilize Devise for authentication purposes.
- Validate all user inputs to prevent any malicious actions and secure the application.
- Choose a view template engine of your choice (.erb, .slim, .haml) to render the views.
- Deploy the project and make it accessible online to facilitate testing and evaluation.

## Database Schema

The database schema should reflect the following structure:

![Database Schema](link-to-your-database-schema-image)

Please note that the "Entity" name mentioned in the schema diagram should be changed according to the theme chosen for your project. It's important to avoid using "Transaction" as the name for your model and table since ActiveRecord already uses it, which would result in an error.

---

Remember to continuously commit your changes using proper gitflow and maintain a professional documentation style throughout your project.
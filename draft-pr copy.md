# Ruby on Rails capstone project - Rails-Wallet Budget-app

## Description

The Ruby on Rails capstone project ([remember what they are?](https://github.com/microverseinc/curriculum-html-css/blob/main/articles/capstone_intro.md)) is about building a mobile web application where we can manage our budget: we have a list of transactions associated with a category, so that we can see how much money we spent and on what. 

We will create a Ruby on Rails application that allows the user to:
- register and log in, so that the data is private to them.
- introduce new transactions associated with a category.
- see the money spent on each category.

**** image model ***

### Project requirements

#### Design
- We should follow these [design guidelines](https://www.behance.net/gallery/19759151/Snapscan-iOs-design-and-branding?tracking_source=), including:
  - Colors.
  - Typography: font face, size and weight.
  - Lawet: composition and space between elements.

The [Creative Commons license of the design](https://creativecommons.org/licenses/by-nc/4.0/) requires that we give appropriate credit to the author. Therefore, we must do it in the README of our project.

#### Interactions
- Splash screen
  - A simple page with the name of our app (yes, we need to choose one), and links to the sign up and log in pages.

- Sign up and log in pages
  - The user should be able to register in the app with full name, email and password (all mandatory).
  - The user can log into the app using email and password.
  - If the user is not logged in, they can't access pages that require the user to be logged in (all the pages described below).

- Home page (categories page)
  - When the user logs in, they are presented with the categories page.
  - For each category, the user can see their name, icon and the total amount of all the transactions that belongs to that category.
  - When the user clicks (or taps) on a category item, the application navigates to the transactions page for that category.
  - There is a button "add a new category" at the bottom that brings the user to the page to create a new category.

- Transactions page
  - For a given category, the list of transactions is presented, ordered by the most recent.
  - At the top of the page the user could see the total amount for the category (sum of all of the amounts of the transactions in that category).
  - There is a button "add a new transaction" at the bottom that brings the user to the page to create a new transaction.
  - When the user clicks on the "Back" button (<), the user navigates to the home page.

- "Add a new category" page
  - The user fills out a form to create a new category, indicating their name and icon (both mandatory).
  - The user clicks (or taps) the "Save" button to create the new category, and is taken to the home page on success.
  - When the user clicks on the "Back" button (<), the user navigates to the home page.

- "Add a new transaction" page
  - The user fills out a form to create a new transaction with:
    - name (mandatory)
    - amount (mandatory)
    - categories (mandatory at least one)
  - The user click (or taps) the "Save" button to create the new transaction, and is taken to the transactions page for that category.
  - When the user clicks on the "Back" button (<), the user navigates to the transactions page for that category.

#### Testing requirements
- Create unit and integration tests for all the most important components of our RoR application.

#### Technical requirements

- We should use Postgres as our database.
- We should use devise for authentication.
- We should validate all user input to make sure that anyone with bad intentions cannot compromise our app.
- We can use a view template engine of our choice (.erb, .slim, .haml).
- The project should be deployed and accessible online.
- our database schema should reflect the following structure:

## Challenge breakdown

Activity list:

- Set up the repository and tools.
- Create our models according to the ERD diagram. Don't forget about validations and tests.
- Implement the authentication and authorization. 

- Create the page to add a category.
- Create the home page.
- Create the page to add a transaction.
- Create the transactions page.

- Make sure our app is tested adequately.
- Deploy the project, and test for final details.
  [Deploy link](https://rails-wallet.onrender.com)
- Record a video for our project.
  [Video link]()
- Create a good README and PR description.

### General requirements (Don't forget)

- Make sure that there are no linter errors.
- Make sure that we used correct gitflow.
- Make sure that we documented our work in a professional way.
- Follow our list of best practices for Ruby.

@ivanmvh
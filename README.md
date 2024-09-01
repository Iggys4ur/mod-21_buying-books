
# Book Buyer

## Project Overview

**Book Buyer** is a web application that allows avid readers to search for books and keep a list of those they are interested in purchasing. The application integrates with the Google Books API to fetch book details and provides a user-friendly interface to save and manage book selections. It is built using the MERN stack (MongoDB, Express.js, React, Node.js) and refactored to utilize GraphQL with Apollo Server for efficient data handling.

## User Story

```md
AS AN avid reader
I WANT to search for new books to read
SO THAT I can keep a list of books to purchase
```

## Acceptance Criteria

```md
GIVEN a book search engine
WHEN I load the search engine
THEN I am presented with a menu with the options Search for Books and Login/Signup and an input field to search for books and a submit button
WHEN I click on the Search for Books menu option
THEN I am presented with an input field to search for books and a submit button
WHEN I am not logged in and enter a search term in the input field and click the submit button
THEN I am presented with several search results, each featuring a book’s title, author, description, image, and a link to that book on the Google Books site
WHEN I click on the Login/Signup menu option
THEN a modal appears on the screen with a toggle between the option to log in or sign up
WHEN the toggle is set to Signup
THEN I am presented with three inputs for a username, an email address, and a password, and a signup button
WHEN the toggle is set to Login
THEN I am presented with two inputs for an email address and a password and login button
WHEN I enter a valid email address and create a password and click on the signup button
THEN my user account is created and I am logged in to the site
WHEN I enter my account’s email address and password and click on the login button
THEN the modal closes and I am logged in to the site
WHEN I am logged in to the site
THEN the menu options change to Search for Books, an option to see my saved books, and Logout
WHEN I am logged in and enter a search term in the input field and click the submit button
THEN I am presented with several search results, each featuring a book’s title, author, description, image, and a link to that book on the Google Books site and a button to save a book to my account
WHEN I click on the Save button on a book
THEN that book’s information is saved to my account
WHEN I click on the option to see my saved books
THEN I am presented with all of the books I have saved to my account, each featuring the book’s title, author, description, image, and a link to that book on the Google Books site and a button to remove a book from my account
WHEN I click on the Remove button on a book
THEN that book is deleted from my saved books list
WHEN I click on the Logout button
THEN I am logged out of the site and presented with a menu with the options Search for Books and Login/Signup and an input field to search for books and a submit button
```

## Features

- **GraphQL Integration:** Refactor from RESTful API to GraphQL for efficient data handling.
- **User Authentication:** Secure user sign-up, login, and logout functionalities.
- **Search Functionality:** Search for books using keywords through the Google Books API.
- **Save Books:** Users can save books to their personal list.
- **Manage Saved Books:** View and remove books from the saved list.

## Technologies Used

- **Front End:** React.js
- **Back End:** Node.js, Express.js, Apollo Server
- **Database:** MongoDB (using MongoDB Atlas)
- **API:** Google Books API
- **Authentication:** JSON Web Tokens (JWT) for secure authentication
- **Deployment:** Render

## Getting Started

### Prerequisites

- Node.js
- MongoDB Atlas account

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/yourusername/book-buyer.git
    ```

2. Navigate into the directory:

    ```bash
    cd book-buyer
    ```

3. Install dependencies:

    ```bash
    npm install
    ```

4. Set up environment variables:

    Create a `.env` file in the root of your project with the following variables:

    ```plaintext
    MONGODB_URI=<your-mongodb-uri>
    JWT_SECRET=<your-jwt-secret>
    ```

5. Start the development server:

    ```bash
    npm start
    ```

6. Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

## Deployment

This application is deployed on Render. You can access the live application [here](#).

## License

This project is licensed under the MIT License.

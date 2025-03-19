# Book Search Engine README

## Project Overview

This Book Search Engine allows users to search for books, save their favorite books to an account, and manage their saved books. It includes login and signup functionality for user accounts and provides an interface for searching books via Google Books API. Users can sign up, log in, search for books, save books to their account, and view or remove saved books.

## Features

- **Book Search:** Allows users to search for books by entering keywords in an input field and viewing a list of books with titles, authors, descriptions, images, and links to Google Books.
- **Login/Signup:** Provides options for users to log in or sign up. Once logged in, users can save books to their account and view their saved books.
- **Saved Books:** Logged-in users can save books to their account and remove them from their saved list.
- **Responsive Interface:** The application dynamically adjusts based on whether the user is logged in or not, offering different menu options accordingly.

## Functional Requirements

### 1. Initial Interface (Not Logged In)
When the user first loads the site:
- The menu will show the following options:
  - **Search for Books**
  - **Login/Signup**
- There will also be an input field to search for books and a submit button.

### 2. Search for Books
- **Search Field:** Users can enter a search term and click the submit button to search for books.
- **Results:** If the user is not logged in, they will see a list of books, each with the following details:
  - Book title
  - Author name
  - Book description
  - Book image
  - Link to the Google Books site

### 3. Login/Signup
- **Login/Signup Modal:** When the user clicks the Login/Signup menu option, a modal appears that allows the user to toggle between login and signup forms.
- **Signup Form:** If the toggle is set to Signup, the user will see the following fields:
  - Username
  - Email address
  - Password
  - Signup button
- **Login Form:** If the toggle is set to Login, the user will see the following fields:
  - Email address
  - Password
  - Login button
- **Account Creation (Signup):** When a valid email and password are entered, the user can click on the signup button, and their account will be created, logging them into the site.
- **User Login:** After entering a valid email address and password, users can log in by clicking the login button, which will close the modal and log the user into the site.

### 4. Menu After Login
Once logged in, the menu will change to the following options:
- **Search for Books**
- **My Saved Books**
- **Logout**

### 5. Save and View Books
- **Save Books:** Logged-in users can save books by clicking the "Save" button on any book search result.
- **Saved Books Page:** Users can view all books they have saved on the "My Saved Books" page, which displays each saved book’s title, author, description, image, and a link to the Google Books site.
  - Each saved book will also have a **Remove** button to delete it from the saved list.

### 6. Logout
- **Logout:** When the user clicks on the Logout button, they will be logged out and the interface will revert to the initial menu with the following options:
  - **Search for Books**
  - **Login/Signup**
  - Input field to search for books
  - Submit button

## Installation Instructions

### Prerequisites
Ensure you have the following installed:
- Node.js (v14 or higher)
- npm (Node Package Manager)

### 1. Clone the Repository
Clone this repository to your local machine using the following command:

```bash
git clone https://github.com/your-username/book-search-engine.git
```

### 2. Install Dependencies
Navigate to the project directory and run the following command to install all dependencies:

```bash
npm install
```

### 3. Start the Development Server
To start the local development server, run:

```bash
npm start
```

This will start the application on `http://localhost:3000` by default.

### 4. Build for Production
To build the application for production, run:

```bash
npm run build
```

This will generate the `build` folder containing the optimized production version of the app.

## API Integration

This project interacts with the **Google Books API** to fetch book data. The search functionality queries this API to display book information, including the title, author, description, and image.

## Future Enhancements

- **User Profile:** Allow users to update their profile details (email, username).
- **Book Ratings:** Enable users to rate and review books.
- **Search Filters:** Implement advanced search filters such as genre, publication date, etc.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Google Books API for providing the data on books.
- React.js for building the user interface.

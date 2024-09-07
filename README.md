## Forkify

![Forkify App Snapshot](https://github.com/user-attachments/assets/af7dfa05-0e69-4bbe-a231-86c389009f22)


### Table of Contents

1. [Description](#description)
2. [Demo](#demo)
3. [Features](#features)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Technologies](#technologies)
7. [Configuration](#configuration)
8. [MVC Architecture](#mvc-architecture)
9. [Disclaimer](#disclaimer)

### Description

Forkify is a JavaScript application that allows users to search for recipes, view detailed information, bookmark their favorite recipes, and even add their own recipes. The app follows the MVC (Model-View-Controller) architecture and interacts with the Forkify API to fetch and manage recipe data.

### Demo

[Link to Demo](https://forkify-alahmady.netlify.app/)

### Features

- **Recipe Search**: Users can search for recipes by entering keywords.
- **Detailed Recipe View**: Displays all the ingredients, cooking instructions, and preparation time.
- **Bookmarking**: Users can bookmark their favorite recipes and access them easily.
- **Pagination**: The app supports pagination for search results, making it easier to navigate through multiple pages.
- **Add Recipes**: Users can add their own recipes to the app.
- **Responsive Design**: The app is designed to be fully responsive and user-friendly on different devices.

### Installation

1. **Clone the repository**:

   ```bash
   git clone https://github.com/Ahmad-AL-Ahmady/your-repository.git
   cd your-repository
   ```

2. **Install necessary dependencies**:

   ```bash
   npm install
   ```

3. **Start the development server**:
   ```bash
   npm start
   ```

### Usage

- **Search for Recipes**: Enter a keyword in the search bar and hit enter. Browse through the results using the pagination controls.
- **View a Recipe**: Click on a recipe from the search results to see detailed information, including ingredients and cooking instructions.
- **Bookmark a Recipe**: Click on the bookmark icon to save a recipe for later.
- **Add a Recipe**: Click on the "Add Recipe" button to open the recipe submission form, fill in the details, and submit.

### Technologies

- **JavaScript (ES6)**: Core logic and functionality.
- **HTML & CSS**: Structure and styling.
- **Forkify API**: Provides recipe data.
- **NPM**: Package management.
- **NPM Libraries**: `parcel`, `fracty`, `core-js`, `regenerator-runtime`

### Configuration

- **API URL**: The app uses the Forkify API to fetch recipe data. The base URL is set in the `config.js` file:
  ```js
  export const API_URL = "https://forkify-api.herokuapp.com/api/v2/recipes/";
  ```
- **Timeout Setting**: Request timeout is set to 10 seconds:
  ```js
  export const TIMEOUT_SECONDS = 10;
  ```
- **Results Per Page**: Controls the number of search results displayed per page:
  ```js
  export const RES_PER_PAGE = 10;
  ```
- **Modal Close Time**: Time (in seconds) before the modal automatically closes:
  ```js
  export const MODAL_CLOSE_SEC = 2;
  ```

### MVC Architecture

- **Model**: Handles data fetching, state management, and business logic. Key functions include loading recipes, managing bookmarks, and handling pagination.
- **View**: Renders UI components and updates the DOM. The app uses multiple views like `recipeView`, `searchView`, `paginationView`, `bookmarksView`, and more to display different parts of the app.
- **Controller**: Serves as the intermediary between the model and view. It orchestrates the app’s logic, listens for events, and triggers updates.

### Disclaimer

This project is based on the coursework provided by [Jonas Schmedtmann](https://github.com/jonasschmedtmann) in his JavaScript course. The HTML and CSS code were written by Jonas Schmedtmann with minor edits by Ahmed AlAhmady.

### Further Reading

- [Jonas Schmedtmann's JavaScript Course](https://www.udemy.com/course/the-complete-javascript-course/)

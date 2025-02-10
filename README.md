# MealDB Food Recipe App

A React-based food recipe application that fetches meal data using Axios from TheMealDB API. This app allows users to browse meal categories, search for meals, and view detailed meal information.

## Features
- 📌 Browse meals by category
- 🔍 Search for recipes
- 📖 View detailed meal descriptions
- ⚡ Fast API calls using Axios
- 🎨 Styled with SCSS
- 🔄 Loading indicator for better UX

## Technologies Used
- React.js
- Axios
- Redux (if applicable)
- React Router
- SCSS for styling

## Installation & Setup

1. Clone the repository:
  
   git clone https://github.com/yourusername/mealdb-food-recipe-app.git
  

2. Navigate to the project directory:

   cd mealdb-food-recipe-app
   

3. Install dependencies:
   
   npm install


4. Start the development server:
   
   npm start
  
   The app will be available at `http://localhost:3000`

## API Integration
This project fetches meal data from [TheMealDB API](https://www.themealdb.com/api.php) using Axios.

### Example API Call (Inside `src/api/axios.js`)
--js
import axios from 'axios';

const API_URL = 'https://www.themealdb.com/api/json/v1/1';

export const fetchMealsByCategory = (category) => {
    return axios.get(`${API_URL}/filter.php?c=${category}`);
};


## Project Structure

mealdb-food-recipe-app/
│-- src/
│   │-- components/
│   │   │-- Category/
│   │   │-- Header/
│   │   │-- Meal/
│   │-- api/
│   │   │-- axios.js
│   │-- actions/
│   │   │-- mealsActions.js
│   │-- App.js
│   │-- index.js
│-- public/
│-- package.json
│-- README.md


## Contributing
Feel free to fork this repository and submit pull requests with improvements. 😊

## License
MIT License


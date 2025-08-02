# Mini React Apps - Student Project

This project contains multiple mini applications built with React and Vite for learning purposes.

## Setup

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start development server:
   ```bash
   npm run dev
   ```

## Project Structure

```
src/
├── apps/           # Mini applications
│   └── RecipeApp.jsx
├── utils/          # Utility functions
│   └── api.js      # API helper functions
├── App.jsx         # Main app component
├── App.css         # Global styles
└── main.jsx        # Entry point
```

## Current Apps

### Recipe App
A simple recipe management application that demonstrates:
- Basic React state management with `useState`
- Form handling and input validation
- Static HTML rendering (hardcoded recipe cards)
- Basic styling with inline CSS

**Features:**
- Add new recipes with title, ingredients, and instructions
- View recipes in card format
- Form validation before adding recipes

## Learning Tasks

### 1. Dynamic Recipe Rendering
Currently, recipes are hardcoded as static HTML. Students should:
- Remove hardcoded recipe cards
- Use the `recipes` state array to dynamically render recipe cards
- Implement `.map()` function to display all recipes
- Make the "Add Recipe" functionality work with the dynamic list

### 2. API Integration
The project includes `src/utils/api.js` with commented API functions. Students should:
- Implement the actual API calls using fetch() or axios
- Replace mock data with real API endpoints
- Add error handling for API failures
- Use `useEffect` to fetch recipes on component mount
- Update state management to work with async API calls

**API Functions to implement:**
- `getRecipes()` - Fetch all recipes from server
- `addRecipe()` - Add new recipe to server
- `deleteRecipe()` - Delete recipe from server

### 3. Express Backend Setup
To create a backend server for your API, students should:

**Backend Setup Steps:**
1. Create a new directory for backend (e.g., `recipe-backend`)
2. Initialize npm project and install Express
3. Set up basic Express server with CORS middleware
4. Create routes for recipe operations (GET, POST, DELETE)
5. Use in-memory array or JSON file for data storage initially
6. Add input validation and error handling middleware
7. Test API endpoints using Postman or similar tools

**Backend Structure Guide:**
- `server.js` - Main server file with Express setup
- `routes/` - API route handlers for different endpoints
- `middleware/` - Custom middleware functions (CORS, validation, etc.)
- `data/` - Data storage (JSON files or database connection)

**API Endpoints to Create:**
- `GET /api/recipes` - Return all recipes
- `POST /api/recipes` - Create new recipe
- `DELETE /api/recipes/:id` - Delete recipe by ID
- `PUT /api/recipes/:id` - Update recipe (optional)

### 4. Enhanced Features
Additional features students can implement:
- Edit existing recipes
- Delete recipes with confirmation
- Search/filter recipes
- Recipe categories
- Image upload for recipes
- Recipe rating system

### 5. Adding New Mini Apps
To add a new mini application:
1. Create a new directory in `src/apps/` (e.g., `src/apps/TodoApp/`)
2. Create the main component file (e.g., `TodoApp.jsx`)
3. Create `utils/api.js` for API functions with TODO comments
4. Use hardcoded HTML instead of dynamic rendering initially
5. Update `src/App.jsx` to import and render the new app
6. Add navigation between different apps

## Code Guidelines

- Use functional components with hooks
- Keep components simple and focused
- Follow React best practices
- Use meaningful variable and function names
- Add comments for complex logic
- Handle errors gracefully

## Next Steps

1. **Make Recipe App Dynamic**: Replace static HTML with dynamic rendering
2. **Connect to API**: Implement real API calls in `utils/api.js`
3. **Add More Apps**: Create additional mini applications
4. **Improve Styling**: Enhance the UI/UX design
5. **Add Testing**: Write unit tests for components

## Resources

- [React Documentation](https://react.dev/)
- [Vite Documentation](https://vitejs.dev/)
- [JavaScript Fetch API](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API)
- [React Hooks](https://react.dev/reference/react/hooks)
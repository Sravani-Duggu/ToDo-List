
# To-Do Application

This is a simple To-Do application built with ReactJS and Redux. It allows users to add, view, mark as completed, and delete tasks. The application also includes persistent storage using local storage, ensuring that tasks are not lost on page reload.

## Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/todo-app.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd todo-app
   ```

3. **Install dependencies:**

   ```bash
   npm install
   ```

## Running the Application

1. **Start the development server:**

   ```bash
   npm start
   ```

   This will run the application in development mode. Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

## How to Use

- **Add Task:** Enter a task in the input field and press Enter or click the "Add Task" button.
- **View Tasks:** All added tasks will be displayed in a list format.
- **Mark as Completed:** Click on a task to mark it as completed. Completed tasks will have a strike-through text style.
- **Delete Task:** Click on the "Delete" button next to a task to remove it from the list.

## File Structure

The project has the following file structure:

```
todo-app/
│
├── public/
│   ├── index.html
│   └── styles.css
│
├── src/
│   ├── components/
│   │   ├── TaskInput.js
│   │   └── TaskList.js
│   ├── redux/
│   │   ├── actions.js
│   │   ├── reducers.js
│   │   └── store.js
│   ├── App.js
│   ├── index.js
│   └── styles.css
│
├── node_modules/
├── package.json
└── README.md
```

## Logic and Approach

The To-Do application is built using ReactJS and Redux, following these principles:

1. **Component Structure:**
   - The application is divided into components to manage different parts of the UI.
   - `TaskInput` component allows users to input new tasks.
   - `TaskList` component displays the list of tasks and allows users to interact with them.

2. **State Management with Redux:**
   - Redux is used to manage the application state, including the list of tasks.
   - Redux actions are dispatched to add, delete, or toggle the completion status of tasks.
   - Reducers handle these actions and update the state accordingly.
   - The application's store is created using `createStore` from Redux, and it maintains the state of the tasks.

3. **Persistent Storage:**
   - Local storage is used to persist tasks between sessions.
   - The application state is serialized and stored in local storage whenever it changes.
   - When the application is loaded, the initial state is retrieved from local storage if available.

4. **Adding, Viewing, Marking, and Deleting Tasks:**
   - Users can add, view, mark as completed, and delete tasks using intuitive user interfaces.
   - Tasks are updated in the Redux store, triggering re-renders to reflect changes in the UI.
   - Completed tasks are visually distinguished with a strike-through text style.

5. **Visual Enhancements:**
   - CSS styles are applied to improve the visual presentation of the application.
   - Components are styled with rounded corners, shadows, and hover effects for better user experience.
   - CSS animations can be added to further enhance the visual appeal of the application.

By following this logic and approach, the To-Do application provides a user-friendly interface for managing tasks efficiently while ensuring persistence and state management using Redux.
```

This README.md file now includes a detailed description of the logic and approach used in developing the To-Do application, providing insights into its architecture and implementation.

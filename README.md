
# Todo App

This is a full-stack Todo application built with the MERN stack (MongoDB, Express, React, Node.js). The application allows users to register, log in, create, update, complete, and delete tasks. It also includes user authentication and authorization using JWT tokens.

## Features

- User Registration and Login
- JWT Authentication
- Create, Read, Update, and Delete (CRUD) tasks
- Mark tasks as complete or incomplete
- Responsive UI with React and Bootstrap
- State management with Redux Toolkit
- API integration with Redux Toolkit Query
- Error handling and notifications with React Toastify

## Technologies Used

- MongoDB
- Express
- React
- Node.js
- Redux Toolkit
- React Router
- React Bootstrap
- Tailwind CSS
- SWR
- Jest and Supertest for testing

## Getting Started

### Prerequisites

- Node.js and npm installed
- MongoDB installed and running

### Installation

1. Clone the repository:

```sh
git clone https://github.com/your-username/todo-app.git
cd todo-app
```

2. Install dependencies for both the backend and frontend:

```sh
npm install
cd frontend
npm install
cd ..
```

3. Create a 

.env

 file in the root directory and add the following environment variables:

```env
NODE_ENV=development
PORT=8000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

### Running the Application

1. Start the backend server:

```sh
npm run server
```

2. Start the frontend development server:

```sh
npm run client
```

3. The application should now be running at `http://localhost:3000`.

### Running Tests

To run the tests, use the following command:

```sh
npm test
```

## Project Structure

```
.
├── backend
│   ├── config
│   │   └── db.js
│   ├── controllers
│   │   ├── taskController.js
│   │   └── userController.js
│   ├── middleware
│   │   ├── authMiddleware.js
│   │   └── errorMiddleware.js
│   ├── model
│   │   ├── taskModel.js
│   │   └── userModel.js
│   ├── routes
│   │   ├── taskRoutes.js
│   │   └── userRoutes.js
│   ├── utils
│   │   ├── generateToken.js
│   │   └── validateToken.js
│   ├── app.js
│   └── tests
│       └── taskRoutes.test.js
├── frontend
│   ├── public
│   │   └── index.html
│   ├── src
│   │   ├── components
│   │   │   ├── Header.jsx
│   │   │   ├── Hero.jsx
│   │   │   ├── Loader.jsx
│   │   │   ├── PrivateRoute.jsx
│   │   │   ├── FormContainer.jsx
│   │   │   ├── EditTodo.jsx
│   │   │   ├── icons
│   │   │   │   ├── DeleteIcon.jsx
│   │   │   │   ├── EditIcon.jsx
│   │   │   │   └── TickIcon.jsx
│   │   │   └── ui
│   │   │       ├── button.jsx
│   │   │       ├── dialog.jsx
│   │   │       ├── input.jsx
│   │   │       └── label.jsx
│   │   ├── screens
│   │   │   ├── HomeScreen.jsx
│   │   │   ├── LoginScreens.jsx
│   │   │   ├── ProfileScreen.jsx
│   │   │   ├── RegisterScreen.jsx
│   │   │   └── Todos.jsx
│   │   ├── slices
│   │   │   ├── apiSlice.js
│   │   │   ├── authSlice.js
│   │   │   └── usersApiSlice.js
│   │   ├── store.js
│   │   ├── App.jsx
│   │   ├── index.css
│   │   ├── main.jsx
│   │   └── lib
│   │       └── utils.js
│   ├── .gitignore
│   ├── package.json
│   ├── postcss.config.js
│   ├── tailwind.config.js
│   └── vite.config.js
├── .gitignore
├── package.json
└── README.md
```

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License.
```
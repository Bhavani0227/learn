ASSIGNMENT TITLE: Redux-based Invoice Management System

PROJECT DESCRIPTION:

The Redux-based Invoice Management System is a web application built using React and Redux. The system allows users to create, view, edit, and delete invoices. It provides a user-friendly interface for managing invoices efficiently.

INSTALLATION AND SETUP INSTRUCTIONS:

To set up the project locally, follow these steps:
Clone the repository from GitHub: [repository link]
Navigate to the project directory.
Install the dependencies by running the command: npm install
Start the development server: npm start
Access the application in your browser at http://localhost:3000.
Live Demo
The application is deployed and can be accessed through the following link: [live demo link]

FUNCTIONALITY:

The application meets the following requirements:
Cloned the GitHub repository and set up the project locally.
Integrated Redux into the application and created a Redux store.
Created Redux actions, action types, and reducers to manage the invoice state.
Implemented a component to display a list of invoices.
Moved the create invoice functionality to a separate create invoice button.
Added buttons/options for view, edit, and delete operations in the invoice list.
Ensured proper state management by connecting components to the Redux store.
Handled errors gracefully.
Wrote clean, well-documented, and modular code.
// invoiceReducer.js
import { ADD_INVOICE, EDIT_INVOICE, DELETE_INVOICE } from '../actions/types';

const initialState = {
  invoices: [],
};

const invoiceReducer = (state = initialState, action) => {
  switch (action.type) {
    case ADD_INVOICE:
      return {
        ...state,
        invoices: [...state.invoices, action.payload],
      };
    case EDIT_INVOICE:
      // Update the invoice with the specified id
      // and return the updated state
      // ...
    case DELETE_INVOICE:
      // Remove the invoice with the specified id
      // and return the updated state
      // ...
    default:
      return state;
  }
};

export default invoiceReducer;

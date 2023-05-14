
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



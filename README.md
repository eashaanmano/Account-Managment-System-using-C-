## About the System

The project is an account management and financial statement maintenance system designed to keep track of funds received, used, disseminated, and donated by an organization. It records transaction details, maintains a budget, and tallies current balances in cash or kind. Users must have appropriate credentials (Administrator or Accountant rights) to access the system. Depending on their access level, a menu of possible actions is displayed, each leading to functions that perform operations on binary files using relevant class objects.

### Features and Functionality

- **Login Interface**: Differentiates between Administrator and Accountant access levels.
- **Access Levels**:
  - Administrator (Superuser)
  - One of the 10 predefined Accountants

#### Administrator Panel/Menu
- Enter Initial Account Details
- Enter Transactions History
- Display Transactions History (Detailed Account Statement)
- Commit Current Transactions to Budget, Expenditure, and Income
- Display Budget, Income, and Expenditure
- Modify Transaction Details
- Display Accountants' Details
- Exit the Application

#### Accountant Panel/Menu
- Display Transactions History (Detailed Account Statement)
- Display Budget, Income, and Expenditure
- Display Accountants
- Exit the Application

## Program Implementation

The system is implemented using Object-Oriented Programming (OOP) concepts, with classes and objects defining transaction properties. File handling with binary files maintains transaction records. Comments throughout the program indicate the functions and needs of each component. The program uses concepts from Computer Science classes XI and XII to ensure good organization and effective OOP.

### Structures and Classes

- **ACCOUNT Structure**: Represents individual accountants’ login credentials (Username and Password).
- **ITEM Structure**: Represents details of any commodity/item purchased or sold by the company.
- **TRANSACTION Class**: Represents details of each financial transaction and performs operations on transactions.

All transactions are stored in a binary file, `CMPNYACC.DAT`, as objects of the `TRANSACTION` class, appended to maintain records of previous transactions. The company’s initial funds and expenditures are stored in another binary file, `ACCDET.DAT`, for cross-checking and maintaining the account balance.
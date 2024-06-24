# Employee Management System

## Overview

The Employee Management System is a Python script that allows users to manage employee records stored in a MySQL database. It provides basic CRUD operations (Create, Read, Update, Delete) for employees, as well as functionality to generate salary slips.

## Requirements

- Python 3.x
- `mysql-connector-python` library (can be installed via `pip install mysql-connector-python`)

## Setup

### Database Setup

1. **MySQL Setup**:
   - Install MySQL Server if not already installed.
   - Create a database named `company` using MySQL client or MySQL Workbench.
   
2. **Schema Setup**:
   - Use the provided `schema.sql` file to create the necessary table structure within the `company` database.
   - Example SQL command to create the `emp` table:
     ```sql
     CREATE TABLE emp (
         empno INT PRIMARY KEY,
         ename VARCHAR(50),
         dept VARCHAR(50),
         salary INT
     );
     ```

### Running the Script

1. Clone or download the project repository to your local machine.

2. Navigate to the project directory.

3. Modify `employee_mgmt.py` to set your MySQL database connection details (`host`, `user`, `password`, `database`).

4. Open a terminal or command prompt.

5. Run the script using the following command:
python scripts/employee_mgmt.py


Choose an option by entering the corresponding number and follow the prompts to perform the desired operation.

### Functionality

- **SHOW EMPLOYEE LIST**: Displays a list of all employees currently stored in the database.
  
- **ADD NEW EMPLOYEE**: Allows the user to enter details for a new employee and adds them to the database.
  
- **SEARCH EMPLOYEE**: Searches for an employee by their employee number and displays their details if found.
  
- **EDIT EMPLOYEE**: Enables editing of an existing employee's department and salary.
  
- **DELETE EMPLOYEE**: Deletes an employee from the database based on their employee number.
  
- **GENERATE PAY SLIP**: Computes and displays a salary slip for a specified employee.

## Notes

- Error handling is minimal in the provided script. Enhance error handling as per your application's requirements.
  
- Ensure proper input validation to prevent SQL injection and other security vulnerabilities.
  
- Customize and extend functionalities as needed for your specific use case (e.g., additional validation, reporting features, etc.).

## Authors

- Replace this section with your information if distributing or sharing modified versions of this script.

## License

- This script is provided under [MIT License](https://opensource.org/licenses/MIT) unless stated otherwise.


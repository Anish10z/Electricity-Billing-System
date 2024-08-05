
# Electricity Billing System

## Overview

The Electricity Billing System is a Java-based application designed to manage electricity billing processes. It provides functionalities for user login, registration, bill generation, deposit and withdrawal of funds, and viewing customer and bill details. The system is integrated with a MySQL database for data management and uses Swing for the graphical user interface.

## Features

- **User Login**: Allows users to log in as Admin or Customer.
- **Signup**: Registers new users into the system.
- **New Customer Add**: Admin can allocate an unique meter number and register a user.
- **Billing**: Admin assign bills to each according the meter rating on prospective months.
- **Consumer Details Enquiry**: Admin has access to all users profile and Billing statuses.
- **Generate Bill**: Generates and displays the electricity bill for a selected meter number and month.
- **Bill Payment**: From user pannel users are able to pay the bill.
- **Customer Details**: Customerscan check only their details.
- **Upadte Details**: User can update their personal details except the name and the allocated meter number.
- **Utility Tools**: Utilty tools like calculator and notebooks are added in both admin and customer pannel for convenience.
## Screenshots
 <p>
  **Login Interface**
<img src="Screenshot/Login.png" alt="Login.jpg" width="600" height="350" >
 **Admin Interface**
<img src="Screenshot/Login.png" alt="Login.jpg" width="600" height="350" >
 <p>

## Prerequisites

- Java Development Kit (JDK) 8 or higher
- MySQL Database
- Required libraries: 
- `net.proteanit.sql` for handling SQL operations in Swing tables
- Swing components for GUI

    ## Installation

    1. **Clone the Repository**:
       ```bash
          git clone https://github.com/yourusername/your-repo.git
        ```
    2. **Setup MySQL Database**:
    - Create a new database named `Bill_system`.
    - Import the database schema and tables. You can use the SQL scripts provided or create tables manually.
    3. **Configure Database Connection**:
     Update the database connection parameters in the `database` class:
     ```bash
     connection = DriverManager.getConnection("jdbc:mysql://localhost:3306/Bill_system","root","yourpassword");
     ```
    4. **Compile and Run**:

     - Open the project in your preferred Java IDE (e.g., IntelliJ IDEA, Eclipse).
     - Compile the project and run the `Splash` class to start the application.

 ## Usage
  **Login**:

 - Open the application and log in using the credentials of an Admin or Customer.
 - Admins can manage customer accounts and view all transactions.
 - Customers can view and manage their own accounts.
**Signup**:

 - Register as a new user by filling in the required details.
 **View & Pay Bill**:
 - Admin can upadte bill by only just putting user meter rating on respective months.
 - Users are able to check bill and pay.  
 **Generate Bill**:

  - Generate and view the bill for a specified meter number and month.
 **View Details**:

 - Use the Deposit Details and Customer Details screens to view and search for specific information.
  ## Files
  - `Splash.java`: 3s splash sceen apears and application starts running.
 - `Login.java`: Handles user login functionality.
 - `Signup.java`: Manages user registration.
 - `main.java`: Provides multiend interface one is for admin and another is for customers.
 - `newCustomer.java`: Adds new customer.
 - `meterinfo.java`: Additional details of allocated meter.
 - `calculate_bill.java`: Calculates and records electricity bills.
 - `deposit_details.java`: Views bills status and transactions details.
 - `customer_details.java`: Access to admin of all customers details.
 - `bill_details.java`: Shows detailed bill information at customer's end.
 - `pay_bill.java`: Interface fo intialize the transaction.
 - `Payment_bill.java`: Open payment site.
 - `generate_bill.java`: Generates and displays bills.
 - `view_information.java`: Displays users personal details.
 - `upadte_information `: Enable user to update their personal data except name and meter_info.
 - `database.java`: Manages database connections and operations.
  ## Database Schema
 Ensure to create the following tables in the Bill_system database:

 - `new_customer`
 - `bill`
 - `meter_info`
 - `tax`
  ## Contributing
 Contributions are welcome! Please open an issue or submit a pull request if you have suggestions or improvements.

  ## License
 This project is licensed under the MIT License - see the [LICENSE](https://choosealicense.com/licenses/mit/) file for details.
# Pharmacy Drug Management System

## Overview
The Pharmacy Drug Management System is a web-based application designed to facilitate the management of drug inventory, orders, and user interactions. It allows customers to register, log in, browse products, place orders, and enables sellers to manage inventory and view orders.

## System Architecture
The system is structured around a Model-View-Controller (MVC) architecture, separating the application logic, user interface, and database interactions. Below are the primary components:

1. **Frontend**: 
   - Developed using JSP (JavaServer Pages) and HTML for dynamic web content.
   - CSS is used for styling the application.
   - Images are utilized to enhance the user interface.

2. **Backend**: 
   - Java serves as the main programming language for server-side logic.
   - The application interacts with the MySQL database to store and retrieve data.

3. **Database**:
   - The system uses a relational database (MySQL) to manage customer, seller, product, inventory, and order information.

### Major Components:
- **Database**: `drugdatabase.sql`
  - Contains SQL scripts to create the database schema and tables for customers, sellers, products, inventory, and orders.
  
- **Web Application Structure**:
  - **Pharmacy-Drug-Management/**
    - The root directory containing all necessary files for the application.

    - **build/**: Contains compiled JSP files and associated resources.
      - `web/`: Holds JSP files and associated resources.
        - **css/**: Stylesheets for various pages.
        - **images/**: Images used in the application.
        - **WEB-INF/**: Configuration files and libraries.
      
      - **dist/**: Contains the packaged WAR file for deployment.
      
      - **nbproject/**: Configuration files for NetBeans project settings.

    - **conf/**: Configuration files for application settings.

    - **Screenshots/**: Contains screenshots of various functionalities within the application.

## Detailed Explanation of Core Components and Modules

### 1. Database (`drugdatabase.sql`)
- Defines the following tables:
  - `customer`: Stores user information.
  - `seller`: Stores seller details.
  - `product`: Contains product information such as name, manufacturer, manufacturing, and expiry dates.
  - `inventory`: Tracks product quantities for each seller.
  - `orders`: Records customer orders, linking them with products and sellers.

### 2. User Interface
- **JSP Pages**:
  - `Homepage.jsp`: The landing page of the application.
  - `Login.jsp`, `Register.jsp`: Pages for user authentication and registration.
  - `AddProduct.jsp`, `UpdateInventory.jsp`: Seller interfaces for managing products and inventory.
  - `Orders.jsp`, `SellerOrders.jsp`: Displays orders placed by customers and sellers, respectively.

- **HTML Files**: Static pages providing structure and layout.
  - `AddProduct.html`, `Index.html`, etc.

- **CSS Styles**: Stylesheets for aesthetic presentation of web pages.
  - Located in the `css/` folder.

### 3. Business Logic
- **Triggers and Procedures**: 
  - SQL triggers are used to automatically update inventory when an order is placed.

### 4. Configuration Files
- `.classpath`, `.project`, and settings under `.settings/` are specific to the development environment .
- `context.xml` in the `META-INF/` folder configures database connection parameters.

## Conclusion
The Pharmacy Drug Management System provides a streamlined solution for managing pharmacy operations, allowing for efficient customer and seller interactions while maintaining accurate inventory records. 

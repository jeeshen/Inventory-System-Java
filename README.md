# Inventory Management System

A console-based inventory management system designed for warehouse operations, supporting product management, stock tracking, order processing, and supplier coordination.

## Features
- User authentication with role-based access (Staff and Supplier accounts)
- Product management with category and supplier associations
- Stock level monitoring and location tracking across warehouse zones
- Purchase order creation and processing
- Shipment tracking and delivery management
- Return handling and refund processing
- Comprehensive reporting system:
  - Stock level reports
  - Movement reports
  - Purchase reports
  - Return reports
- Transaction logging and audit trails
- Real-time inventory updates and notifications

## Installation
```bash
# clone the repo
git clone https://github.com/yourusername/inventory-management-system.git

# navigate to project directory
cd inventory-management-system

# compile the project using Maven
mvn clean compile

# run the application
mvn exec:java -Dexec.mainClass="Main"
```

## Requirements
- Java 21 or higher
- Maven 3.6 or higher

## Usage
1. Run the application
2. Login with your credentials (Staff or Supplier account)
3. Navigate through the menu system to:
   - Manage products and categories
   - Process orders and shipments
   - Track stock movements
   - Generate reports
   - Handle returns

## Data Files
The system uses the following text files for data persistence:
- `category.txt` - Product categories
- `product.txt` - Product information
- `stock.txt` - Stock levels and locations
- `stockrecord.txt` - Stock movement history
- `order.txt` - Purchase orders
- `shipment.txt` - Shipment details
- `shipmenttracking.txt` - Delivery tracking
- `transaction.txt` - Transaction logs
- `staff.txt` - Staff accounts
- `supplier.txt` - Supplier accounts

## Project Structure
```
src/main/java/
├── Main.java                 - Application entry point
├── Account.java             - User account base class
├── Staff.java               - Staff account management
├── Supplier.java            - Supplier account management
├── Category.java            - Product category management
├── Product.java             - Product management
├── Stock.java               - Stock level management
├── StockRecord.java         - Stock movement records
├── StockLocation.java       - Warehouse location mapping
├── Location.java            - Location entities
├── Order.java               - Purchase order processing
├── Shipment.java            - Shipment management
├── ShipmentTracking.java    - Delivery tracking
├── Transaction.java         - Transaction logging
└── Reports/
    ├── Report.java          - Base report class
    ├── StockLevelReport.java
    ├── MovementReport.java
    ├── PurchaseReport.java
    └── ReturnReport.java
```

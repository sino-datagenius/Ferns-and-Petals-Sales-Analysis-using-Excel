# Data Dictionary

## Product Table Columns

| Column Header | Description |
|---------------|-------------|
| Product_ID | Unique identifier for each product |
| Product_Name | Name/title of the product |
| Category | Type of product (Soft Toys, Plants, Colors, etc.) |
| Price (INR) | Cost in Indian Rupees |
| Occasion | Target celebration/event for the product |
| Description | Brief product details/features |

## Customer Table Columns

| Column Header | Description |
|---------------|-------------|
| Customer_ID | Unique identifier for each customer (C001, C002, etc.) |
| Name | Customer's full name |
| City | Customer's city of residence |
| Contact_Number | Customer's phone number |
| Email | Customer's email address |
| Gender | Customer's gender (Male/Female) |
| Address | Customer's complete postal address |

## Order Table Columns

| Column Header | Description |
|---------------|-------------|
| Order_ID | Unique identifier for each order |
| Customer_ID | Reference to the customer who placed the order |
| Product_ID | Reference to the product being ordered |
| Quantity | Number of items ordered |
| Order_Date | Date when the order was placed |
| Order_Time | Time when the order was placed |
| Delivery_Date | Date when the order was delivered |
| Delivery_Time | Time when the order was delivered |
| Location | Delivery location/city |
| Occasion | Event/celebration for which the order was placed |

## Table Relationships

- **Customer_ID** in the Order table references **Customer_ID** in the Customer table
- **Product_ID** in the Order table references **Product_ID** in the Product table
- This creates a relational database structure linking customers to their orders and ordered products

## Notes

- All ID fields serve as primary keys in their respective tables
- Date fields follow DD-MM-YYYY format
- Time fields follow HH:MM:SS format (24-hour)
- Currency is in Indian Rupees (INR)

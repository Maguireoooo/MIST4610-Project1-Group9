# MIST4610-Project1-Group9

# Team Name:
Group 9
# Team Members:
1. Colin Maguire @Maguireoooo
2. Aidan Brown @breadwinner222
3. Will Shimmons @WillShimmons
4. Sidhant Arora @SidhantArora4610
# Problem Description:
Our flower shop management system is designed to track sales, inventory, suppliers, customers, and employees in a retail flower business. This complex system helps managers efficiently manage orders, keep up with stock, enhance supplier relationships, encourage employee performance, and improve customer spending to maximize profitability and streamline our operations.​
# Data Model:

Our data model assists us in the daily management of a flower shop, and is specialized in dealing with customers, inventory, sales, and employees.

Customer data, which includes names, contact details, and addresses, is maintained in the Customers table, and excels at simplifying the tracking of buyers and their orders.

The Flowers table is able to show the price, stock quantity, and catalog all available flowers, specifying what type of flower it is, such as Roses, Lilies, or Orchids. Each flower is connected to a supplier, whose information is kept in the Suppliers table, which also includes contact details.

The Orders table tracks customer purchases, containing the customer, order date, total price, and status (Pending, Completed, Canceled). Since a single order can include multiple flowers, the Order_Details table links orders to specific flowers and records details like quantity and price.

The Employees table tracks shop workers, including attributes like names, job positions (Florist, Cashier), and salaries. Although they are not directly linked to sales, employees are essential in managing orders and helping customers.

Through the connection of these tables, our flower shop is able to manage inventory, maintain supplier relationships, process customer orders, and see all employee information.


<img width="649" alt="Screenshot 2025-03-12 at 10 25 50 PM" src="https://github.com/user-attachments/assets/c6956e77-c507-403f-bc13-cb1ff3a16d9b" />

# Data Dictionary:
Order_details table:

<img width="624" alt="Screenshot 2025-03-12 at 10 18 36 PM" src="https://github.com/user-attachments/assets/2366d7a6-aea7-405e-93ec-c2acd0612606" />

Orders table:

<img width="627" alt="Screenshot 2025-03-12 at 10 18 06 PM" src="https://github.com/user-attachments/assets/4637916d-b0f0-4e1f-9cca-927c4738e637" />

Employee table:

<img width="623" alt="Screenshot 2025-03-12 at 10 17 44 PM" src="https://github.com/user-attachments/assets/b0fbc5d9-8a2f-4017-bcf9-1a814e3a68d1" />

Flowers table:

<img width="627" alt="Screenshot 2025-03-12 at 10 17 21 PM" src="https://github.com/user-attachments/assets/fd6b1b2d-51f7-4439-9909-51605ff423bc" />

Supplier table:

<img width="614" alt="Screenshot 2025-03-12 at 10 16 52 PM" src="https://github.com/user-attachments/assets/d4640128-ef64-40a9-930b-62ce8799a7f9" />

Customers table:

<img width="621" alt="Screenshot 2025-03-12 at 10 16 22 PM" src="https://github.com/user-attachments/assets/ad7fefc0-b869-4829-841b-2da54cef495e" />

# Queries:
Simple Queries:

1. Retrieves the name and price of each flower from the "flowers" table. Flower names are then listed in order of highest to lowest price. Managers would use this query for basic inventorying purposes. 

2. Creates a new variable that lists the revenue that each flower produces. This is done by joining the flower and order details tables using the respective foreign key and multiplying "flower price" from the flower table by "quantity" from the order details table. Managers use this to track which products are most popular; adjusting costs to meet demand. 

3. 

   
<img width="625" alt="Screenshot 2025-03-12 at 10 29 41 PM" src="https://github.com/user-attachments/assets/5990671c-5e0a-499a-9bcb-ef25ddbb996d" />
<img width="621" alt="Screenshot 2025-03-12 at 10 30 09 PM" src="https://github.com/user-attachments/assets/8607968d-02c3-493a-8545-62d8dcef144f" />

Complex Queries:

1. Combines data from the "Orders" and "Customers" table through the customer_id column; listing the top three customers who have spent over $55. The customers shown are the companies "most valuebale customers." Used to strenghten customer relationships; incentives can be given to these customers to reward loyalty and motivate future business. 

<img width="618" alt="Screenshot 2025-03-12 at 10 30 31 PM" src="https://github.com/user-attachments/assets/fdc2da11-5813-4c3f-8508-c8db00e71cbc" />

2. This query retrieves data from the "Employees" and "Orders" tables, identifying the top three employees who have handled the most orders. It provides insights into employee performance by counting the number of orders each employee has managed. This information can be used for performance evaluations, incentive programs, or workload balancing.


<img width="632" alt="Screenshot 2025-03-12 at 10 30 54 PM" src="https://github.com/user-attachments/assets/fd033012-9017-4a17-8515-b37940eec1af" />

3. This query retrieves data from the "Suppliers" and "Flowers" tables to identify the top three suppliers based on the number of flowers they provide to the shop. By summing the total flower quantity supplied by each vendor, the business can determine its most valuable suppliers, ensuring strong relationships and efficient inventory management.


<img width="620" alt="Screenshot 2025-03-12 at 10 31 15 PM" src="https://github.com/user-attachments/assets/d13e0236-ef99-4f0d-999f-0a22ca1fc0c5" />

# Database Information:
(Not sure what to put here)

file:///var/folders/8y/7sqt3q594vz5pw6mg5vg0pkm0000gn/T/TemporaryItems/NSIRD_screencaptureui_YTWu5g/Screenshot%202025-03-14%20at%209.50.52%E2%80%AFPM.png

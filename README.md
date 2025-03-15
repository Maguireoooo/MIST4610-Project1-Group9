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
<img width="625" alt="Screenshot 2025-03-12 at 10 29 41 PM" src="https://github.com/user-attachments/assets/5990671c-5e0a-499a-9bcb-ef25ddbb996d" />

2. Creates a new variable that lists the revenue that each flower produces. This is done by joining the flower and order details tables using the respective foreign key and multiplying "flower price" from the flower table by "quantity" from the order details table. Managers use this to track which products are most popular; adjusting costs to meet demand. 
<img width="621" alt="Screenshot 2025-03-12 at 10 30 09 PM" src="https://github.com/user-attachments/assets/8607968d-02c3-493a-8545-62d8dcef144f" />

3. This Query shows all the customer details including their names, phone numbers, emails, and their addresses. This helps managers access customer information for processing orders quickly enough to improve their customer service. This also helps build long-term relationships with their customers, as it helps speed up their process.
   
![Simple Query 3](https://github.com/user-attachments/assets/66241763-da14-4bae-94a7-6b8439e93c88)

4. This last simple query allows all the orders to be listed with their ID, date, total price, and be sorted from newest to oldest as well as their status. This helps managers keep an organized record of transactions ensuring smooth business operations and addressing issues without delay.
   
![Simple Query 4](https://github.com/user-attachments/assets/66fed7bf-be21-4fe8-a0e4-86ac888e6b93)


   

Complex Queries:

1. Combines data from the "Orders" and "Customers" table through the customer_id column; listing the top three customers who have spent over $55. The customers shown are the companies "most valuebale customers." Used to strenghten customer relationships; incentives can be given to these customers to reward loyalty and motivate future business. 

<img width="618" alt="Screenshot 2025-03-12 at 10 30 31 PM" src="https://github.com/user-attachments/assets/fdc2da11-5813-4c3f-8508-c8db00e71cbc" />

2. This query retrieves data from the "Employees" and "Orders" tables, identifying the top three employees who have handled the most orders. It provides insights into employee performance by counting the number of orders each employee has managed. This information can be used for performance evaluations, incentive programs, or workload balancing.


<img width="632" alt="Screenshot 2025-03-12 at 10 30 54 PM" src="https://github.com/user-attachments/assets/fd033012-9017-4a17-8515-b37940eec1af" />

3. This query retrieves data from the "Suppliers" and "Flowers" tables to identify the top three suppliers based on the number of flowers they provide to the shop. By summing the total flower quantity supplied by each vendor, the business can determine its most valuable suppliers, ensuring strong relationships and efficient inventory management.


<img width="620" alt="Screenshot 2025-03-12 at 10 31 15 PM" src="https://github.com/user-attachments/assets/d13e0236-ef99-4f0d-999f-0a22ca1fc0c5" />

4. This first complex query finds the top 3 best selling flowers and adds up their total quantity that is sold. This helps managers understand which flowers are popular in their customers. This helps to adjust their inventory levels and focus on high-demand products rather than flowers that don’t leave the shelves for months. This would also allow for more stock space on the flowers that sell more.

![Complex Query 4](https://github.com/user-attachments/assets/82fb2907-3cba-4fb2-a87a-a46b267af142)

5. The fifth query lists employees who earn more than the company’s average salary, sorting it from most to least. This allows managers to analyze the salary distribution and make sure there is fair compensation among their employees. An added benefit of this identifies the employees who are above average, assessing their performance and closely monitoring promotions.

![Complex Query 5](https://github.com/user-attachments/assets/b40f230e-9787-43cd-ade0-b3e0363e71ce)

6. This last query finds the top five employees by tracking highest prices on orders they handled. This also allows the managers to recognize their top employees who are responsible enough to bring large sales, and can be rewarded, improving the sales of the company and motivating the employees who continue to put the effort.

![Complex Query 6](https://github.com/user-attachments/assets/a9161eee-bcbe-44f2-8079-c89b9ebc59b3)



# Database Information:
![Database Information](https://github.com/user-attachments/assets/d542b278-b205-4287-9f5f-a37bcbc4f9dd)

Name of the database: ha_group9

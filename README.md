#Bamazon

Synopsis

An interactive shopping node app where MySQL and Node.JS are used to allow users to purchase items as a customer, view, track and update the product inventory as a manager, and track the total sales by department as a supervisor.

Bamazon Customer Portal

The Bamazon Customer Portal allows users to view the current items available for purchase. 
The user will be prompted to enter the item id# and how many items they wish to purchase. 
If the item is in stock, the order will be completed and the user will see the total amount of their purchase.

David@LAPTOP-A9AM2G9M MINGW32 /c/nodejs/Github/Bamazon (master)
$ node bamazonCustomer
+--------------------------------------------------------------+
¦ Item Id# ¦ Product Name                              ¦ Price ¦
+----------+-------------------------------------------+-------¦
¦ 12345    ¦ Duvet Cover                               ¦ 89.99 ¦
+----------+-------------------------------------------+-------¦
¦ 67891    ¦ Mens Zip-up Hoodie                        ¦ 29.99 ¦
+----------+-------------------------------------------+-------¦
¦ 23456    ¦ Glass Catch-all Dish                      ¦ 15.99 ¦
+----------+-------------------------------------------+-------¦
¦ 34567    ¦ High Rise Skinny Jeans - Black            ¦ 59.99 ¦
+----------+-------------------------------------------+-------¦
¦ 89123    ¦ Womens Bruce Springsteen Baseball T-shirt ¦ 25.99 ¦
+----------+-------------------------------------------+-------¦
¦ 45678    ¦ Mens Knit Beanie - Blue                   ¦ 21.99 ¦
+----------+-------------------------------------------+-------¦
¦ 91234    ¦ Striped Jersey Cotton Sheets - Queen      ¦ 49.99 ¦
+----------+-------------------------------------------+-------¦
¦ 56789    ¦ Spiked Dog Leash                          ¦ 25.99 ¦
+----------+-------------------------------------------+-------¦
¦ 11234    ¦ Shark Kitty Bed                           ¦ 59.99 ¦
+--------------------------------------------------------------+
prompt: Please enter the ID # of the item you wish to purchase!:  34567
prompt: How many items would you like to purchase?:  3

3 items purchased
High Rise Skinny Jeans - Black 59.99
Total: 179.97

Your order has been processed.  Thank you for shopping with us!

------------------------------------------------------------------------------------------
The Bamazon Manager Portal allows users to view and edit the inventory of the store. 
The user will be prompted to choose from the following options:

View products for sale
View low inventory
Add to inventory
Add a new product

Manager Options 1 & 2

The first option allows the user to see the list of products that are currently for sale, 
what department the item belongs to, the price of the product and how much stock is left for that product.

The second option allows the user to see a list of all inventory items that have less than 35 items in stock.
If there are no products that meet this criteria, the user will see an empty table.

David@LAPTOP-A9AM2G9M MINGW32 /c/nodejs/Github/Bamazon (master)
$ node bamazonManager
prompt: Key in one of the following options: 1) View Products for Sale 2) View Low Inventory 3) Add to Inventory 4) Add New Product:  1

Products for Sale

+-------------------------------------------------------------------------------------------------+
¦ Item Id# ¦ Product Name                              ¦ Department Name ¦ Price ¦ Stock Quantity ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 12345    ¦ Duvet Cover                               ¦ Home            ¦ 89.99 ¦ 25             ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 67891    ¦ Mens Zip-up Hoodie                        ¦ Mens Clothing   ¦ 29.99 ¦ 25             ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 23456    ¦ Glass Catch-all Dish                      ¦ Home            ¦ 15.99 ¦ 5              ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 34567    ¦ High Rise Skinny Jeans - Black            ¦ Womens Clothing ¦ 59.99 ¦ 27             ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 89123    ¦ Womens Bruce Springsteen Baseball T-shirt ¦ Womens Clothing ¦ 25.99 ¦ 5              ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 45678    ¦ Mens Knit Beanie - Blue                   ¦ Mens Clothing   ¦ 21.99 ¦ 5              ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 91234    ¦ Striped Jersey Cotton Sheets - Queen      ¦ Home            ¦ 49.99 ¦ 10             ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 56789    ¦ Spiked Dog Leash                          ¦ Pets            ¦ 25.99 ¦ 10             ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 11234    ¦ Shark Kitty Bed                           ¦ Pets            ¦ 59.99 ¦ 5              ¦
+-------------------------------------------------------------------------------------------------+

David@LAPTOP-A9AM2G9M MINGW32 /c/nodejs/Github/Bamazon (master)
$ node bamazonManager
prompt: Key in one of the following options: 1) View Products for Sale 2) View Low Inventory 3) Add to Inventory 4) Add New Product:  2

Items With Low Inventory

+-------------------------------------------------------------------------------------------------+
¦ Item Id# ¦ Product Name                              ¦ Department Name ¦ Price ¦ Stock Quantity ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 12345    ¦ Duvet Cover                               ¦ Home            ¦ 89.99 ¦ 25             ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 67891    ¦ Mens Zip-up Hoodie                        ¦ Mens Clothing   ¦ 29.99 ¦ 25             ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 23456    ¦ Glass Catch-all Dish                      ¦ Home            ¦ 15.99 ¦ 5              ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 34567    ¦ High Rise Skinny Jeans - Black            ¦ Womens Clothing ¦ 59.99 ¦ 27             ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 89123    ¦ Womens Bruce Springsteen Baseball T-shirt ¦ Womens Clothing ¦ 25.99 ¦ 5              ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 45678    ¦ Mens Knit Beanie - Blue                   ¦ Mens Clothing   ¦ 21.99 ¦ 5              ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 91234    ¦ Striped Jersey Cotton Sheets - Queen      ¦ Home            ¦ 49.99 ¦ 10             ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 56789    ¦ Spiked Dog Leash                          ¦ Pets            ¦ 25.99 ¦ 10             ¦
+----------+-------------------------------------------+-----------------+-------+----------------¦
¦ 11234    ¦ Shark Kitty Bed                           ¦ Pets            ¦ 59.99 ¦ 5              ¦
+-------------------------------------------------------------------------------------------------+

Manager Options 3 & 4

The third option allows the user to update the inventory for a specific product. 
A prompt asks what the id is for the product the user wants to update. 
A second prompt asks how many items the user wishes to increase the quantity by.

The last option allows the user to add a new product to the inventory. 
Prompts ask the user for the product id#, the product name, the department name, the price and the stock quantity.

David@LAPTOP-A9AM2G9M MINGW32 /c/nodejs/Github/Bamazon (master)
$ node bamazonManager
prompt: Key in one of the following options: 1) View Products for Sale 2) View Low Inventory 3) Add to Inventory 4) Add New Product:  3
prompt: What is the ID number of the product you want to add inventory for?:  23456
prompt: How many items do you want to add to the inventory?:  100

The new updated stock quantity for id# 23456 is 105

+----------------------------------------------------------------------------+
¦ Item Id# ¦ Product Name         ¦ Department Name ¦ Price ¦ Stock Quantity ¦
+----------+----------------------+-----------------+-------+----------------¦
¦ 23456    ¦ Glass Catch-all Dish ¦ Home            ¦ 15.99 ¦ 105            ¦
+----------------------------------------------------------------------------+

David@LAPTOP-A9AM2G9M MINGW32 /c/nodejs/Github/Bamazon (master)
$ node bamazonManager
prompt: Key in one of the following options: 1) View Products for Sale 2) View Low Inventory 3) Add to Inventory 4) Add New Product:  4
prompt: Please enter a unique 5 digit item Id #:  54321
prompt: Please enter the name of the product you wish to add:  Floor Lamps
prompt: What department does this item belong in?:  Home
prompt: Please enter the price of the item in the format of 00.00:  39.99
prompt: Please enter a stock quantity for this item:  200

New Item Added

+--------------------------------------------------------------------+
¦ Item Id# ¦ Product Name ¦ Department Name ¦ Price ¦ Stock Quantity ¦
+----------+--------------+-----------------+-------+----------------¦
¦ 54321    ¦ Floor Lamps  ¦ Home            ¦ 39.99 ¦ 200            ¦
+--------------------------------------------------------------------+

David@LAPTOP-A9AM2G9M MINGW32 /c/nodejs/Github/Bamazon (master)
$ node bamazonSuper
prompt: Key in one of the following options: 1) View Product Sales by Department 2) Create New Department:  1

Product Sales by Department

+------------------------------------------------------------------------------+
¦ Department ID ¦ Department Name ¦ Overhead Cost ¦ Total Sales ¦ Total Profit ¦
+---------------+-----------------+---------------+-------------+--------------¦
¦ 1             ¦ Mens Clothing   ¦ 10000         ¦ 219.9       ¦ -9780.1      ¦
+---------------+-----------------+---------------+-------------+--------------¦
¦ 2             ¦ Pets            ¦ 10000         ¦ 0           ¦ -10000       ¦
+---------------+-----------------+---------------+-------------+--------------¦
¦ 3             ¦ Home            ¦ 20000         ¦ 79.95       ¦ -19920.05    ¦
+---------------+-----------------+---------------+-------------+--------------¦
¦ 4             ¦ Shoes           ¦ 15000         ¦ 0           ¦ -15000       ¦
+---------------+-----------------+---------------+-------------+--------------¦
¦ 5             ¦ Electronics     ¦ 50000         ¦ 0           ¦ -50000       ¦
+---------------+-----------------+---------------+-------------+--------------¦
¦ 6             ¦ Womens Clothing ¦ 25000         ¦ 179.97      ¦ -24820.03    ¦
+------------------------------------------------------------------------------+

David@LAPTOP-A9AM2G9M MINGW32 /c/nodejs/Github/Bamazon (master)
$ node bamazonSuper
prompt: Key in one of the following options: 1) View Product Sales by Department 2) Create New Department:  2
prompt: Please enter the name of the new department you would like to add.:  Sporting Goods
prompt: What are the overhead costs for this department?:  5000.00

New Department sucessfully created!


David@LAPTOP-A9AM2G9M MINGW32 /c/nodejs/Github/Bamazon (master)

Technologies Used:

* Javascript
* nodeJS
* MySQL
* npm packages:
	mysql
	prompt
	colors/safe
	cli-table









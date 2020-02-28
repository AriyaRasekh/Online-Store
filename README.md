# Online-Store

# Scenario:

A retail store wants to build an online system for their customer to place orders online and for pickup later
from the store.
Customers join the system by registering online (username (email), password, address, phone no) and
including a credit card for use in online ordering; at that time they use login credentials (uername and
password) to enter the online system.
Customers who have joined the system can use the online system to search for products, select products,
specify amounts or weights for products where necessary, and place orders for those products, specifying a
pick-up time. (The system enforces a 24-hour minimum pick-up time). When an order has been placed,
an email confirming its receipt and listing order details is sent to the customer. (The customer have the
opportunity to edit their order for a certain period of time). When an order is received by the system it is
forwarded to order processors, who collect and package up the ordered items, and sends an email confirming
the completion of the order to the customer. The customer go to the store in the chosen pick-up time, call a
number to inform his arrival, and waiting to the designated area. Cashier charges the customers’ credit card
appropriately and deliver the order. Customers can use the on-line system to check past orders, to inquire
into order statuses, and take a short survey after every order. The system logs information on all orders,
containing details on what was ordered, charges, and order status.
One alternative scenario is worth noting. When customers order products, they are allowed to order
only products (or amounts of products) that are currently present in inventory. When order processors are
processing orders, however, inventory may have changed, and certain products (or requested amounts of those
products) may no longer be available. Such products are omitted from the orders, or supplied to the extent
possible. Such cases are noted and inform (by email and a phone call) to the customer. The customer is not
charged for such items. Another alternative scenario is if customers do not show up in the chosen pick-up
time, they will be charged based on their delay.


# Actors: 
Customer, System Processor, Cashier, Tax agency

# Use cases: 
-	Registration:  get customer’s Full name and email address, if the email address if already exists, show a message and go to login page, if it’s new email, ask for password, address, Credit card information & phone no, if Address, Credit card or phone No is not valid, Show an error massage.
-	Login: Ask for an Email address as Username and password, if Email does not exist, go to registration page, if password doesn’t match the account, show invalid Email/Password error message, after few times of entering invalid Email/Password, send an email to username with resetting password instruction.

-	Searching Items: Allow customers to search for Item with name, ID, price ranges and weight if applicable.

-	Choosing Items: Adding Item’s to cart, show final price plus tax and shipping( if applicable), and how many lefts in the inventory.

-	Placing order: Finalize their purchase after customer selected the Item, update inventory.

-	Pick up: Ask the customer to choose from specific locations, and time to pick up the Item, pick up time should be at least 24 hours after placing the order.

-	Receipt: Order processor sends an Email with the receipt as proof of purchase with detail of Item such as price, name ID and pick up detail.

-	online order logging : system logs customer’s orders, containing order details, charges and order status and history

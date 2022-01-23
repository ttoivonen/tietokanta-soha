# **Order-to-Cash application**

The purpose of the application is to manage a sales cycle (of physical goods), also known Order to Cash. The users can manage the whole cycle from placing an order to receiving payment from the customer. The process flow consists of:
1. Customer Service placing an Order to a customer: Order to document is created in Orders table
2. Logistics creates a delivery for an open Order: Delivery document is created in Deliveries table
3. Invoicing creates an Invoice for delivered goods: Invoice document is created in Invoices table
4. Invocing receives customer's payment for the Invoice: payments is created to Payments table

The below picture describes the conceptual model of the application.


The application uses the following tables to store data:
- Customers_MD: Master Data of Customers, e.g. customer name, address etc.
- Materials_MD: Materia Master Data for existing materials, table holds e.g. unit price of a material
- Users_MD: Master Data of users, e.g. name, roles
- Roles_MD: Master Data table for roles in the application, e.g. authorization for invoicing
- Orders: table stores created Orders with their data
- Deliveries: table for deliveries, i.e. outbound movement of goods
- Invoices: invoices issues to customer, e.g. net amount, status if the invoice is paid
- Payments: table collects customer payments for invoices

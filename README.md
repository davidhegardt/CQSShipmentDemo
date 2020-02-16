# CQSShipmentDemo
Demonstration of CQS pattern with a Shipment Order Service.
Not to be used or redistributed. Client app removed on purpose.
Compiled files removed, this is for demonstration purpose only
and probably won't run out of the box :).

Application Simulates a Shipping management system using CQS pattern
with MediatR libary using Commands (Process) and Queries.

Application uses localDB and seeds data with the following properties:

Shipment - Contains Orders 
Orders - Contains Items 
Items - the shipped goods and its quantity

Shipment has MANY orders PK = ShipmentID
Orders has MANY items PK = OrderID FK = ShipmentID
Items has ONE Order PK = ItemID FK = OrderID

Ef Core sets up these relationships automatically in this model first approach.
+ All code written and implemented by David Hegardt

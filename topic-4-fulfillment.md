Topic 4 --- Fulfillment
=======================

### Basic fulfillment process

1. `SALES` receive **purchase order** from `CUST`
2. `SALES` create **sales order**
	- then sends to `WAREHOUSE`
3. `WAREHOUSE` prepares **shipment**
4. `WAREHOUSE` sends **shipment** to `CUST`
5. `ACCT` creates **invoice**
	- then sends to `CUST`
6. `ACCT` receives **payment** from `CUST`

### Organizational data used in fulfillment process

1. Client
2. Company code
3. Sales organization
	- like P Org but for sales
4. Division
	- `1..*` S Org : `1..*` Division relationship
	- used to group FERTig / HAndelsWaren materials with similar characteristics
5. Distribution channel
	- Modes of distribution:
		- Wholesale
		- Retail
		- Internet
6. Sales area
	- A composition of all the permutations of which the sales organizations, divisions and distribution channels are linked
7. Plant of which the product to-go is currently housed in
8. Storage location (within the plant)
9. Shipping point
	- Physical location from which the products are to be shipped from
		- Loading dock
		- Mail room
		- Rail depot
		- Employees in charge of handling expedited orders
10. Credit control area

	- `1..*` Plant : `1..a
	- One or more organizations responsible for managing customer credit limits
	- Customer credit limits = maximum amount of money a customer can owe (i.e. invoice sent to customer, but customer hasn't paid)
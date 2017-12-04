Topic 4 --- Fulfillment
=======================

## Fulfillment Proeess

### Overview

1. `SALES` receive **purchase order** from `CUST`
2. `SALES` create **sales order**
	- then sends to `WAREHOUSE`
3. `WAREHOUSE` prepares **shipment**
4. `WAREHOUSE` sends **shipment** to `CUST`
5. `ACCT` creates **invoice**
	- then sends to `CUST`
6. `ACCT` receives **payment** from `CUST`

### Technically accurate

1. Pre-sales activity
	- Necessary advertisement, marketing and contact points enable receive a purchase order
2. Sales order processing
3. Inventory sourcing
4. Shipping
5. Billing
6. Payment

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
	- One or more organizations responsible for managing customer credit limits
	- Customer credit limits = maximum amount of money a customer can owe (i.e. invoice sent to customer, but customer hasn't paid)
	- `1..*` Plant : `1..*` CCA relationship

## Master Data
- Material master
	- General data
	- Accounting / Financial data (company-level data)
	- Sales-specific data (sales-area-level data)
- **Customer master**
	- **4 Partner functions:**
		- **Sold-to-party** (Legal ownership)
		- **Ship-to-party** (Who actually received it)
		- **Bill-to-party** (Legal paying party)
		- **Payer**			(Who actually paid for it)
	- **3 Customer data types [MCQ](#problematic-mcq):**
		+ **General**
		+ **Financial Accounting**
		+ **Sales Area**
		+ Think: "Vendor Master", but instead of Purchasing data for the purchasing organization, it is sales area data for the sales organization
- Customer-material info record
	- Associates material and customer master data
- **Pricing Conditions**
	- **Material price**
	- **Customer specific price**
	- **InCoTerms (International commercial terms)**
	- **Surcharges / discounts**
	- **Taxes**
- Output master data
	- e.g. quotation, order confirmation, invoices
	- includes which media used to transmit the output:
		- e.g. Mail, fax, EDI
- Credit management master record
	- General data (client-level)
		- Total credit at enterprise level
	- Credit control area level
		- Credit limit per credit control area
		- Risk category
		
## **Pre-sales activity**

Required activity before the fulfillment process can logically be proceeded with:

- Creating and tracking customers (contacts)
- Mailing Campaigns (**advertisement**)
- Responding to **customer inquiries and RFQ**
- Sending back the **quotations**
- Outline agreements
	+ Contracts
	+ Scheduling agreements

## Sales Order Processing

**Data to put in sales order:**

- Customer data
- Material data
- Pricing conditions
- Shipping information
- Billing information

## Deliveries

**Multiple sales order can be compounded into a single delivery**

**IF the following are common**
- customer
- delivery date
- shipping point (from dock/airport/rail)
- ship-to-address (to dock/airport/rail)

(One sales order may be split up into several deliveries)


## Post Goods Issue

> Goods Issue is Posted once the FERTig goods left the warehouse / plant on the way to the customer

**What happens when Post Goods Issue:**

- A material document is created
- General Ledger accounts (Stock & cost of goods sold) updated
- Accounting document created
- COntrolling document created
- Billing due list is updated
- Sales documents are updated

## Credit Management Process

> Process which determines if credit (i.e. debt to the organization) should be granted to customer

### MCQ

*"The customer credit management process assesses whether credit should be granted when:"*

- Sales order is created/changed
- Delivery is created/changed
- Goods Issue is Posted


## Problematic MCQ

*"Which of the following key organizational elements are unique to the fulfillment process?"*
: **Sales area**
: **Credit control area**
: **Shipping point**

*"In the fulfillment process, a plant is..."*
: **A facility from which the company delivers products and services to its customers**

*"	The three segments into which the data in the customer master are divided are ________"*
: **Financial accounting data**
: **Sales area data**
: **General data**

*"The customer credit management process assesses whether credit should be granted when:"*
: **Sales Order created/changed**
: **Delivery created/changed**
: **Posting Goods Issue**
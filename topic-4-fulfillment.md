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
		- **Sold-to-party**
		- **Ship-to-party**
		- **Bill-to-party**
		- **Payer**
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


## Impact of Post Goods Issue

- A material document is created
- General Ledger accounts (Stock & cost of goods sold) updated
- Accounting document created
- COntrolling document created
- Billing due list is updated
- Sales documents are updated
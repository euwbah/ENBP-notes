Topic 3 -- Procurement
====================

## Steps of procurement:

1. Create purchase requisition
2. Create & send purchase order
3. Receive materials => `out` Goods receipt -> Goods Movement => `out` Material document
4. Receive invoice
5. Invoice verification
6. Send payment

## Data required in the procurement process

### Organizational Data

1. Client
2. Company Code (belongs to client)
3. Plant (belongs to company)
4. Storage Location (within plants)
5. [Purchasing organization](#purchasing-organization)
6. Purchasing Group

### Master Data

- Material Master
- **Vendor Master**
	1. General Data    (Client-level data)
	2. Accounting Data (Company-level data)
	3. Purchasing Data (P Org-level data)
- Purchasing Info Record
	- Associative type between Material & Vendor Master
	- **Conditions**
		- Gross price
		- Discounts, surcharges
		- Frieght / shipping costs
	- Conditions obtained from
		- Purchasing info records
		- Contracts & agreements
		- Other sources
		
## Item Categories

: Defines the process used to procure / means of which the item is procured

1. Standard
2. Subcontracting
	- ROH/HALB sent, FERT received
3. Consignment
	- These goods are sent over & delivered, but still owned by the vendor until sold by the company
4. Service
5. Stock transfeer
6. Third party order
	- Product shipped to third-party, but cost is paid by first-party

## Stock Types

: Defines how the material can be used

1. Unrestricted use
	- This is the only type of stock that can be sent to customers in the fulfillment process
2. In quality inspection
3. Blocked stock
4. Stock in transit

## Purchasing Organization

### Roles of a purchasing organization:

1. Identify & select vendors
2. Negotiate general conditions of purchase
3. Negotiate pricing

### Three purchasing organization models:

1. Enterprise-level:
	- cross-company-code model
	- one POrg for all CC and plants
	- centralized & corporate

2. Company-level:
	- cross-plant model
	- one POrg per CCWhich element of a purchase order includes communicating with the vendor?

3. Plant-level:
	- plant-specific model
	- one POrg per plant
	- decentralized

**Reference purchasing organization**
: One enterprise-level Ref. POrg for high-level decisions collating company-level &|/ plant-level POrgs
: Usage scenarios:
- to collate multiple lower-level POrg's orders into a single order in the event that buying in a larger quantity would warrant a better price per item
- for sake of contract
- for abstraction's sake

### *vs.* Purchasing Group

A purchasing **group** is the buyer/group of buyers responsible for the execution of the actual purchase, a purchasing **organization** simply decides whether, what, and from where / who to buy.

## Purchase Order

### MCQ

*"Which element of a purchase order includes communicating with the vendor?"*
: Outcome

### Steps to create one:

1. Trigger
	- Purchase requisition
	- RFQ
	- Quotation
	- Another Purchase Order
2. Data
	- Master Data
	- Transaction documents
	- User input
3. Task
	- Determine vendor (if unknown)
	- Create purchase order
4. Outcome
	- Results in a purchase order (duh)
	- Update purchase requisition
	- **Communicate with vendor**
	
## Goods receipt

Outcomes:
- Material Documents created
- Accounting Documents created
- Material Master update
- PO history update
- Quality management performed

	
## Invoice Verification

### MCQ

*"Which of the following documents are required for the invoice verification step of the procurement process?"*
: Vendor invoice
: Purchase order
: Material document

## Tested topics

- Organizational Data (Slide 6)
- Purchasing organization role & responsibilities & level names
- The 4 Master Data in the procurement process
- Vendor Master's 3 levels
- Conditions
- Item Categories
- Stock Types
- Goods Receipt (Maybe)

## Problematic MCQs

*Which of the following is(are) a form of data within the goods receipt step?*
: All of the above

*Which one of the following is not a model of the purchasing organization?*
: Client-level (The correct term is Enterprise-level PO)

*What is a storage location?*
: The place within a plant where materials are kept until they are needed
: *think __generic__*

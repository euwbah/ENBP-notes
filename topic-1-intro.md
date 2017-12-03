Topic 1 --- Introduction
=======================

**What is an Enterprise System?**
: An enterprise system supports and integrates business process so that different sectors/function groups/sub-companies of the company/enterprise need not manually tally their database, stocks, assets and infrastructure

**What is an Enterprise Resource Planning System?**
: It **is an Enterprise System** which relates to the **internal operations** of an enterprise, which **integrates functional and cross-functional** business processes.
SAP is an example of an ERP System, which additionally is fully *`l10n`-ized* in terms of language and currency support.

### 3 benefits of an Enterprise System

1. Increased productivity
2. Increased profitability
3. Competitive edge

### Material Types

**ROH**stoffe -> Raw stuff

**HALB**fabrikat -> Half-fabricated (Semi-finished goods)

**HA**ndels**WA**ren -> Handling wares (Trading goods)

**FERT**ig -> Finished

### Data types:

1. **Organizational Data**
	
	Something like metadata...
	Represents company objects in a hierarchical manner
	
	Client > Comapny > Plant
	
	> Client (The group of companies, i.e. the enterprise, the yiffmedaddy)
	> Company codes (Each company is in charge of some plants)
	> Plants (A plant can relate to one or more business processes/functions)

2. **Master Data**

	models & database
	> Customer
	> Vendor
	> Materials
	>
	> Master data, like transaction data, are a consequence of executing process steps. However, note that
	> <marquee><h2 style="background-color:#c0eeff"> <u>IT IS NOT CONSTANTLY CHANGING</u> </h2></marquee>

3. **Situational Data**

	implied associative types
	> who
	> when
	> where

4. **Transaction Data**
    
    The culmination of all the data working in tandem,
    being the epitome of all *"associative types"*
    > *"__Transaction data__ reflects the consequences of executing process steps"*
    
### Documents

Documents are **records of transactions**

Types of documents:

1. Transaction Documents
	- Purchase Requisition & Order, Invoice, Delivery Document
2. FInancial Documents
	- Shows impact on finnancial accounting
3. COntrolling Documents
	- Shows impact on management accounting (how the company should organize & develop itself)
4. Material Documents
	- Shows impact on quantity, status, location of material
# Topic 5: Production

## The Production Process

- *Warehouse* requests **Production**
- *Production* authorizes **Production**
- *Warehouse* issues **Raw materials**
    + i.e. **Goods Issued**
- *Production* creates **Product**
    + i.e. **Goods Receipt**
- *Warehouse* receives **Finished Goods**

## Master Data

### Bill Of Materials

+ **BOM Structure (IMPORTANT!)**:x
    * Header:
        - Status: Active | Inactive
        - Base Quantity
        - Usage: Production | Engineering | Costing
        - Plant
        - Validity
    * Items:
        - Material Number
        - Quantity
        - Item Category - either...
            + Stock Item - Must have material master
            + Nonstock item - No material master
            + Variable-sized item - Must specify size
            + Document item - diagrams, additional instructions

### Work Center

+ **Data about production operations/activities**
+ Work centers can represent:
    * Employees involved in production process
    * (Unmovable) Machines
    * Assembly Lines
+ Includes...: (not important)
    * Basic Data
        - Name
        - Description
        - Person in charge of maintaining master data
        - Task list usage - which routings can use this work center
    * Capacities
    * Scheduling
    * Cost Center
    * Human Resource assignment
        - Employees Names & Shifts

### Product Routing

+ **Represents a series of sequential operations that must be carried out in the process of producing that product**
+ Consists of (important??):
    * Operations
    * Sequence
        - Standard
        - Alternate
        - Parallel
    * Work center
    * Times (duration)
        - Setup, Machine, Labor

![Routing](pics/routing.png)
            
### Material Master (not important)

**Specific to production:**
- **Work Scheduling**
- **Material Resource Planning**

and the others...

- Basic Data
- Purchasing-related data
- Sales-related data
- Accounting related data

### Production Resource Tools

> Basically any **portable/movable** items that is required in the production process

- Instruction Documents
- Materials
- Equipment
- Miscellaneous

This is unlike **static unmovable machinery** that should be classified under **[Work Centers](#work-center)** instead.

### Things to study

- Basic Production Process
- Goods Issued -> Issue raw material for prod    
- Goods Receipt -> Transfer the goods produced to warehouse
- Master Data (All)
- BOM Struct
- Work Center
- Routing
- Material Master
- Production Resource Tool (PRT)
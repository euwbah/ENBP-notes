# Topic 3: Procurement

### Filling in a Purchase Order

**Reorder pt**
: When stock quantity == reorder pt, order x amount of stock where x == order quantity

**Order quantity**
: The de-facto quantity to buy when restocking once qty hits reorder point

> Remember to read the question carefully! Some questions will ask only to sum up invoice from a **certain** vendor only


## The Procurement Process

1. *Warehouse* creates **purchase requisition**
2. *Purchasing organization* sends **purchase order**
3. *Warehouse* receives **materials**
    - **Goods Receipt Step**
        + _"More inventory = more assets"_
        + Financial Impact
            * **Inventory** in debit (+ve value)
            * **GR/IR (goods-receipt/invoice-receipt) clearing account** in credit (in debt)
                - **Think: _"awaiting invoice"_**. The GR/IR clearing account keeps track of how much is in credit when the goods are received (GR) but the invoice hasn't been sent yet.
        + Material Impact
            * Items delivered
4. *Accounting organization* receives **invoice**
    - **Invoice Verification Step**
        + _"More liabilities (owings/debits)"_
        + Financial Impact
            * **GR/IR clearing account** is balanced (debit is set to the value of credit in the goods receipt step)
            * **Vendor** and **Accounts Payable (A/P)** in credit (debted to the vendor)
5. *Accounting organization* sends **payment**
    - **Payment Processing Step**
        + _"Pay up liabilities, bank money fly"_
        + Financial Impact
            * **Vendor** and **Accounts Payable (A/P)** credits will be balanced with debit after payment is done.
            * **Bank account** will be in credit (debt to the bank)
        + **IMPORTANT Final outcome:**
            * Inventory in debit step 1
            * GR/IR credit in ste/p 1 then balanced in step 2
            * Vendor & A/P in credit in step 2 then balanced in step 3
            * Bank in credit in step 3

## Organizational Data

- Plant
- Storage Location
- Purchasing Organization
    + 3 self-explanatory levels that differ in degrees of centralization:
        * Enterprise-level
        * Company-level
        * Plant-level

## Master Data

- Material Master
- Vendor Master
- Purchasing Info Record (The associative entity between **materials** & **vendors**)
- **Pricing Conditions IMPORTANT**
    + Includes these 3 factors:
        * Gross price (original price)
        * Discounts & surcharges
        * Freight / shipping charges
    + Derived from
        * **Purchasing Info Record**
        * Contracts & Agreements
        * Any other sources

## Key concepts

- **Item Categories IMPORTANT**
    + i.e. the **process** of which the item is procured
        * Standard
        * Subcontracting (Give components to vendor, they build the finish product for a fee)
        * Consignment (Only credit/liable/indebted to vendor when the good is withdrawn from stock - i.e. used)
        * Service
        * Stock transfer
        * Third party order (Ship to them, but bill to us; order on behalf of other party)
- Account determination
- Stock type/status
- **Goods movement IMPORTANT**
    + Goods Receipt
        * The act of receiving of goods from vendor
    + Goods Issue
        * The act of exporting goods to customer or for internal consumption
    + Stock Transfer
        * Physical movement of material
    + Transfer Posting
        * Changing Material Status (unrestricted use/in quality inspection/blocked)
        * Change in physical location is not mandatory

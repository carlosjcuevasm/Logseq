- Catalog
- Inventory
- Orders
- Invoices
- Payments
- Shipping
-
- Most often an ERP-lite approach is best. Companies have solutions in place and you need to assembly around them for the best solution.
- It means:
	- Not forcing a massive ERP rollout
	- Using **just enough ERP**
	- Integrating tools instead of replacing them
	- ntegrating tools instead of replacing them
-
- ## Catalog vs Inventory vs Invoicing (they are NOT the same)
- People casually mix these up, but in business systems they’re **distinct layers**.
-
- ### 🟦 Catalog —  *What you sell*
  This answers:
- What products/services exist?
- Name, description, SKU
- Price (maybe)
- Categories
- Images/specs
  
  A catalog can exist **without selling anything**.
- Examples:
- PDF price list
- Website product list
- WooCommerce in “catalog mode”
  
  👉 **Catalog = marketing + reference**
- ---
- ### 🟩 Inventory —  *What you physically have*
  
  This answers:
- How many units exist?
- Where are they?
- Reserved vs available
- Low-stock alerts
  
  Inventory is **stateful** and changes constantly.
  
  👉 **Inventory = operational reality**
  
  ---
- ### 🟨 Invoicing —  *What was sold*
  
  This answers:
- What was sold
- To whom
- When
- For how much
- Taxes, discounts, payment status
  
  An invoice is a **legal/accounting document**.
  
  👉 **Invoice = financial record**
-
- ### Key insight (very important)
  
  > 
  
  **An invoice does NOT update inventory by magic unless the system is wired correctly.**
  
  That wiring is what “inventory sync” means.
-
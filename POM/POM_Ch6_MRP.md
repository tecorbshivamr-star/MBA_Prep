# 📗 POM CHAPTER 6: Aggregate Planning, MPS & MRP
### Subject: Production & Operations Management | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

Imagine you manage a factory making Air Conditioners (ACs). 
- In Winter, nobody buys ACs. 
- In Summer, everyone buys ACs. 

How do you plan your production for the year?
- **Option 1 (Chase):** Fire all your workers in Winter. Hire hundreds of temporary workers in Summer. (Cheap on inventory, but bad for morale and training costs).
- **Option 2 (Level):** Keep the same 100 workers all year. Produce 1,000 ACs every month. In Winter, you store the unsold ACs in a massive warehouse. In Summer, you sell out the warehouse. (Good for workers, but warehouse costs are huge).

This is **Aggregate Production Planning (APP)**—planning the big picture for the next 6-12 months.

---

## 🟡 INTERMEDIATE LEVEL — "Key Concepts & Frameworks"

### 1. The Planning Hierarchy (Zooming In)
1. **Aggregate Plan:** "We will make 12,000 Air Conditioners this year." (High-level, long-term).
2. **Master Production Schedule (MPS):** "We will make 200 Window ACs in Week 1, and 300 Split ACs in Week 2." (Zoomed in, detailed by specific product and week).
3. **Material Requirements Planning (MRP):** "To make 200 Window ACs next week, the computer says we need to order exactly 200 compressors and 800 screws *today* so they arrive on time." (Zoomed in to the raw material level).

### 2. MRP (Material Requirements Planning)
MRP is software logic. It needs 3 things to work:
1. **The MPS:** Tells the computer what finished goods to make.
2. **Bill of Materials (BOM):** The "recipe." It tells the computer that 1 AC = 1 compressor + 1 fan + 4 screws. 
3. **Inventory Records:** The computer checks the warehouse. "We need 400 screws, but we have 100 in stock. Therefore, we only need to order 300."

---

## 🔴 ADVANCED / EXAM LEVEL — "How to write it in the exam?"

### Q. What is Aggregate Production Planning? Differentiate between the 'Chase' and 'Level' strategies. What are the key inputs required for an MRP system? (15 Marks)

**1. Definition of Aggregate Production Planning (APP):**
Aggregate Planning is a medium-term capacity planning technique (typically covering 3 to 18 months) that determines the optimal combination of production rate, workforce level, and inventory on hand to meet fluctuating demand. It is called "aggregate" because it does not deal with specific individual products (e.g., red cars vs blue cars), but rather an aggregate unit of output (e.g., "total cars").

**2. Chase vs. Level Strategy:**

| Feature | Chase Strategy | Level Strategy |
| :--- | :--- | :--- |
| **Core Concept** | Match the production rate exactly to the demand rate period by period. | Maintain a constant production rate and a constant workforce level all year. |
| **How it handles fluctuations** | By aggressively hiring and firing workers, or using overtime and subcontracting. | By using inventory as a buffer (building up stock during low demand, depleting it during high demand). |
| **Major Costs Incurred** | High HR costs (hiring, training, severance pay, loss of morale/quality). | High inventory holding costs (warehousing, insurance, obsolescence risk). |
| **Best Suited For** | Service industries (where inventory cannot be stored, e.g., restaurants hiring extra staff on weekends) or industries where holding costs are exorbitant. | Capital-intensive manufacturing (where idle machines cost millions) and products with low holding costs. |

**3. Material Requirements Planning (MRP) & Its Inputs:**
While APP plans the "big picture" months in advance, MRP is the computerized information system that schedules the day-to-day ordering of the actual raw materials and components needed to execute the plan. 
MRP acts as a giant calculator, working backwards from the delivery date, using lead times to determine exactly *when* to place an order.

**The Three Essential Inputs for MRP:**
*   **A. Master Production Schedule (MPS):** Derived from the Aggregate Plan, it details exactly how many specific end items (finished goods) are to be produced and on what specific dates.
*   **B. Bill of Materials (BOM):** The engineering document showing the hierarchical product structure. It lists every single sub-assembly, component, and raw material required to build one unit of the finished good (like a recipe card).
*   **C. Inventory Record File (IRF):** The real-time database showing exactly how much of every component is currently sitting in the warehouse (On-Hand), and how much has already been ordered and is in transit (Scheduled Receipts), along with the lead time for each part.

**Conclusion:**
By integrating the MPS, BOM, and Inventory data, the MRP system generates "Planned Order Releases," ensuring that manufacturing never stops due to missing parts, while simultaneously preventing excess capital from being tied up in unnecessary raw material inventory.

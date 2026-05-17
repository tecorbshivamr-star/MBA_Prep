# 📗 POM CHAPTER 5: Inventory Management
### Subject: Production & Operations Management | MBA 2nd Semester | DU SOL
**From Beginner → Exam Ready**

---

## 🟢 BEGINNER LEVEL — "What is this about?"

**Inventory** is just money sitting in a warehouse disguised as raw materials or finished boxes. 
- If a smartphone company has 1 Lakh unsold phones in a warehouse, that's ₹200 Crores of cash locked up. The phones might get stolen, damaged, or become outdated (obsolete). This is the **Cost of Holding Inventory**.
- But if they have 0 phones in the warehouse, and a customer walks in to buy one, the customer walks away angry. This is the **Cost of a Stockout**.

Inventory Management is the mathematical art of keeping *just enough* stock to keep customers happy, without going bankrupt from warehouse costs.

---

## 🟡 INTERMEDIATE LEVEL — "Key Concepts & Frameworks"

### 1. The Two Opposing Costs
1. **Ordering Costs:** Every time you place an order, you pay for transport, truck unloading, and administrative paperwork. If you order small amounts very often, this cost explodes.
2. **Holding (Carrying) Costs:** If you order one massive shipment per year (to save on transport), you need a giant warehouse, security guards, and insurance. Your holding cost explodes.

### 2. Economic Order Quantity (EOQ)
This is the magic formula that perfectly balances the two costs above. It tells you exactly how many units to order at one time to achieve the lowest possible total cost.
> **EOQ = √(2DS / H)**
*(D = Annual Demand, S = Setup/Ordering Cost, H = Holding Cost per unit).*

### 3. ABC Classification
You cannot treat a ₹1 lakh car engine and a ₹1 screw the same way.
- **'A' Items (Vital):** Make up 80% of your total inventory value, but only 20% of the quantity. (e.g., Engines). You track these daily with high security.
- **'C' Items (Trivial):** Make up 5% of the value, but 50% of the quantity. (e.g., Screws, rubber bands). You just buy a huge bin of them and forget about them until the bin is empty.

---

## 🔴 ADVANCED / EXAM LEVEL — "How to write it in the exam?"

### Q. Explain the concept of Economic Order Quantity (EOQ) with its underlying assumptions. A firm requires 12,000 units of a raw material per year. The ordering cost is ₹100 per order, and holding cost is ₹2.40 per unit per year. Calculate the EOQ and the number of orders per year. (15 Marks)

**1. Concept of EOQ:**
Economic Order Quantity (EOQ), developed by Ford W. Harris, is a fundamental inventory control model. It determines the optimal order size that minimizes the Total Annual Inventory Cost (which is the sum of Total Ordering Cost and Total Holding Cost). At the exact EOQ point, the Annual Ordering Cost is perfectly equal to the Annual Holding Cost.

**2. Assumptions of the Basic EOQ Model:**
While mathematically elegant, EOQ relies on strict, idealized assumptions:
*   Demand (D) is known, constant, and independent.
*   Lead time (time from placing the order to receiving it) is known and constant.
*   Receipt of inventory is instantaneous (the entire batch arrives at once).
*   Quantity discounts are not available (purchase price is constant).
*   Stockouts are completely avoided.

**3. Numerical Solution:**

**Step A: Extract the Data**
*   **D (Annual Demand)** = 12,000 units
*   **S (Ordering/Setup Cost)** = ₹100 per order
*   **H (Holding/Carrying Cost)** = ₹2.40 per unit per year

**Step B: Calculate Economic Order Quantity (EOQ)**
*   Formula: $EOQ = \sqrt{\frac{2 \times D \times S}{H}}$
*   $EOQ = \sqrt{\frac{2 \times 12,000 \times 100}{2.40}}$
*   $EOQ = \sqrt{\frac{2,400,000}{2.40}} = \sqrt{1,000,000}$
*   **EOQ = 1,000 units**
*   *(Interpretation: To minimize total costs, the firm should place an order for exactly 1,000 units every time it buys this raw material).*

**Step C: Calculate Number of Orders per Year**
*   Formula: $Number\ of\ Orders = \frac{Annual\ Demand\ (D)}{EOQ}$
*   Number of Orders = 12,000 / 1,000
*   **Number of Orders = 12 orders per year** (i.e., exactly one order per month).

**Step D: Prove Total Cost is Minimized (Optional but impressive in exams)**
*   Annual Ordering Cost = 12 orders × ₹100 = ₹1,200
*   Annual Holding Cost = (Average Inventory) × H = (EOQ / 2) × 2.40 = (1,000 / 2) × 2.40 = 500 × 2.40 = ₹1,200
*   *(Notice how Ordering Cost exactly equals Holding Cost. This mathematically proves 1,000 is the correct EOQ).*

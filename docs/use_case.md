## **Business Use Case** 

## **Actors**

| **Actor** | **Role Description** |
|:-----------|:---------------------|
| **owner (Admin)** | Oversees inventory control, manages product data, monitors stock levels, and ensures availability for sales. |
| **employee** | Interacts with customers, records sales, and provides product information based on available stock. |

---

## **Use Cases for owner**

#### **Use Case 1: Manage Product Inventory**

| **Element** | **Description** |
|:-------------|:----------------|
| **Goal** | To efficiently manage product data — adding, updating, or removing items from inventory. |
| **Preconditions** | owner has administrative access to the inventory system. |
| **Postconditions** | Inventory is updated; new products become visible to the team; deleted items are removed. |
| **Business Value** | Ensures accurate and up-to-date stock data. |

---

#### **Use Case 2: Monitor Stock Levels**

| **Element** | **Description** |
|:-------------|:----------------|
| **Goal** | To view and track stock availability and identify when to restock. |
| **Preconditions** | Inventory data is available and regularly updated. |
| **Postconditions** | owner has insights into low-stock or high-demand items. |
| **Business Value** | Prevents stockouts and overstocking, optimizing storage and sales. |

---

#### **Use Case 3: View and add Transactions**

| **Element** | **Description** |
|:-------------|:----------------|
| **Goal** | To be able to view and add sales and purchase transactions. |
| **Preconditions** | Transaction data is stored in the system. |
| **Postconditions** | The owner is able to view the transactions of self and the employee. |
| **Business Value** | Supports data-driven decision-making and strategic planning. |

---

## **Use Cases for employee**

#### **Use Case 1: View Available Stock**

| **Element** | **Description** |
|:-------------|:----------------|
| **Goal** | To view available products and their stock levels before interacting with customers. |
| **Preconditions** | Valid login credentials; system connected to live inventory. |
| **Postconditions** | Accurate product and stock information displayed to the employee. |
| **Business Value** | Enables efficient and informed sales interactions with customers. |

---

#### **Use Case 2: Record Sales**

| **Element** | **Description** |
|:-------------|:----------------|
| **Goal** | To record product sales and automatically update stock levels. |
| **Preconditions** | Product must exist in inventory with sufficient quantity. |
| **Postconditions** | Transaction saved; stock reduced accordingly. |
| **Business Value** | Ensures stock accuracy and sales tracking. |

---

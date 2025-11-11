## **Business Use Case** 

## **Actors**

| **Actor** | **Role Description** |
|:-----------|:---------------------|
| **Admin** | Has full control over the system, including managing user accounts (creating or removing managers and salespersons), overseeing inventory, updating stock quantities, recording purchase transactions, and viewing all sales and purchase activities. |
| **Manager** | Oversees inventory control, manages product data, monitors stock levels, and ensures availability for sales. |
| **Salesperson** | Interacts with customers, records sales, and provides product information based on available stock. |

---

## **Use Cases for manager**

#### **Use Case 1: Manage Product Inventory**

| **Element** | **Description** |
|:-------------|:----------------|
| **Goal** | To efficiently manage product data — adding, updating, or removing items from inventory. |
| **Pre conditions** | manager has administrative access to the inventory system. |
| **Post conditions** | Inventory is updated; new products become visible to the team; deleted items are removed. |
| **Business Value** | Ensures accurate and up-to-date stock data. |

---

#### **Use Case 2: View Stock Levels**

| **Element** | **Description** |
|:-------------|:----------------|
| **Goal** | To view and track stock availability and identify when to restock. |
| **Pre conditions** | Inventory data is available and regularly updated. |
| **Post conditions** | manager has insights into low-stock or high-demand items. |
| **Business Value** | Prevents stockouts and overstocking, optimizing storage and sales. |

---

#### **Use Case 3: View and add Transactions**

| **Element** | **Description** |
|:-------------|:----------------|
| **Goal** | To be able to view and add purchase transactions. |
| **Pre conditions** | Transaction data is stored in the system. |
| **Post conditions** | The manager is able to view the transactions of self and the salesperson. |
| **Business Value** | Supports data-driven decision-making and strategic planning. |

---

## **Use Cases for salesperson**

#### **Use Case 1: View Available Stock**

| **Element** | **Description** |
|:-------------|:----------------|
| **Goal** | To view available products and their stock levels before interacting with customers. |
| **Pre conditions** | Valid login credentials; system connected to live inventory. |
| **Post conditions** | Accurate product and stock information displayed to the salesperson. |
| **Business Value** | Enables efficient and informed sales interactions with customers. |

---

#### **Use Case 2: Record Sales**

| **Element** | **Description** |
|:-------------|:----------------|
| **Goal** | To record product sales and automatically update stock levels. |
| **Pre conditions** | Product must exist in inventory with sufficient quantity. |
| **Post conditions** | Transaction saved; stock reduced accordingly. |
| **Business Value** | Ensures stock accuracy and sales tracking. |

---

# **Overview**

Welcome to the documentation of Inventory Management System.

# **Inventory Management System (IMS)**

## **1. Introduction**

The **Inventory Management System (IMS)** is designed to streamline and simplify the management of products, sales, and purchases in grocery marts. These businesses are typically operated by a **manager** who supervises a few **salesperson** responsible for day-to-day operations.  

This document outlines the behaviour of the IMS explaining how different users — **manager** and **salesperson** — interact with the system, what functionalities are available to them, and how the system responds to their actions.  
The purpose is to ensure a clear understanding of the **system’s overall functionality**, helping to align its features with both **user needs** and **business goals**.

---

## **2. Problem Statement**

In many small and medium-sized grocery marts, inventory is still managed **manually** using ledgers, spreadsheets, or informal records. This manual process leads to:  

- Frequent **data inconsistencies** and **human errors**  
- Difficulty in tracking **stock levels** and **product movements**  
- Lack of visibility into **sales and purchase history** 
- Inefficient communication  

As a result, businesses often struggle with **overstocking**, **stockouts**, and **loss of sales opportunities**, impacting both profitability and operational efficiency.

---

## **3. Proposed Solution**

The **Inventory Management System (IMS)** provides a **centralized digital platform** that automates and simplifies inventory-related processes. It enables both manager and salesperson to manage transactions, view stock details, and generate reports efficiently.

### **Key Features**
- **User Roles:** Separate access levels for admins and employees  
- **Product Management:** Add, update, and view product details  
- **Transaction Management:** Record and track **sales** transactions  
- **Stock Tracking:** Updates on product quantities after each transaction  
- **Data Insights:** View historical data   

### **System Benefits**
- Eliminates manual record-keeping and minimizes human errors  
- Improves visibility of stock movement and sales data  
- Ensures accountability through role-based permissions  
- Enhances operational efficiency and decision-making for business growth  

---


## **Objectives**

The primary objectives of the Inventory Management System are:

- **Efficient Stock Management**  
  To provide a platform where admins can add, update, or delete product information and track stock quantities.
- **Role-Based Control**  
  To ensure that access privileges are granted according to user roles (Admin or employee).
- **Transaction Tracking**  
  To maintain a record of all sales transactions.
- **Improved Visibility**  
  To allow visibility of all the products available, making it easier for the employee to interact with customers.
- **Error Reduction**  
  To minimize manual entry errors and duplication by automating stock updates after each transaction.



## **User Roles and Permissions**

The Inventory Management System (IMS) defines three primary user roles — **Admin**, **Manager**, and **Salesperson** — each with distinct levels of access and responsibility. This role-based access control ensures data integrity, operational efficiency, and accountability within the system.

| **Role**       | **Permissions / Capabilities** |
|----------------|--------------------------------|
| **Admin**      | - Can add users.<br>- Can add roles.<br>|
| **Manager**    | - Oversees inventory.<br>- Add, update, or delete products as required.<br>- Update inventory quantities.<br>- View sales transactions made by all salespersons.<br> |
| **Salesperson** | - View available products and their current quantities.<br>- Record sales transactions.<br>- View and track their own transaction history.<br>- Maintain accurate sales entries. |


# **Future Scope**

The Inventory Management System (IMS) in its current version provides a solid foundation for managing products, transactions, and user roles. However, several enhancements are planned to further expand its capabilities.

### **Dashboard Enhancements and Analytics**
Future updates will introduce advanced visual analytics for the admin dashboard. Administrators will be able to view detailed visualizations of purchase and sales data from the previous month, including interactive graphs and trend summaries. These insights will enable better performance monitoring and strategic decision-making. Over time, additional filtering and comparative visualization features may also be integrated to allow detailed exploration by date range, product category, or employee activity.

### **Automated Stock Management**
The system will include automated low-stock alerts to notify administrators when product quantities drop below a defined threshold. This feature will support proactive restocking and prevent stockouts that may affect sales continuity. Alerts may later be extended to include supplier integration for faster replenishment.


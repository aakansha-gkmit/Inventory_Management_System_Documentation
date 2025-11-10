# **Functional Documentation**

## **Introduction**

This document outlines the **functional behavior** of the Inventory Management System (IMS) from the **end-user’s perspective**.  
It describes how users — **owners (Admins)** and **employees** — interact with the system, what functionalities are available to them, and how the system responds to their actions.

The goal is to provide a clear understanding of the **system’s functionality**, ensuring that each feature aligns with user needs and business objectives.

---

## **Functional Requirements — Owner**

#### **1. Login**
- The owner logs into the system using valid credentials.
- The owner enters their username and password, then clicks the **Login** button.
- The system Verifies credentials and grants access to the owner dashboard.  
- This ensures secure access to administrative functionalities.

---

#### **2. Manage Products**

- The owner can view, add, update, or delete products from the inventory.
- The owner navigates to the **Product Management** section to use options such as **Add Product**, **Edit**, or **Delete**
- The system adds, updates or deletes the product.
- This Provides full control over product inventory.

---

#### **3. Add / View Transactions**
- The owner can record new transactions for purchases or sales.  
- The owner navigates to the **Transactions** section and selects **Add Transaction** to record data.  
- The system saves new transaction data and automatically updates stock quantities.  
- The owner can view previous transaction records in the **View Transactions** section.  
- This enables effective tracking of all business operations.  

---
#### **Onwer Flow Overview**

![Owner Flowchart](assests/images/owner.svg){ style="display:block; margin-left:auto; margin-right:auto;"}

## **Functional Requirements — Employee**

#### **1. Login**
- The employee logs into the system using valid credentials.  
- The employee enters their username and password, then clicks the **Login** button.  
- The system validates the credentials and grants access to the employee dashboard.  
- This ensures secure access control and prevents unauthorized usage.  

---

#### **2. View Products and Details**
- The employee can view all available products along with their details such as name, quantity, and price.  
- The employee navigates to the **Products** section to browse the available stock.  
- The system displays a list of products with their details but restricts editing or deletion.  
- This allows the employee to assist customers efficiently based on real-time stock information.  

---

#### **3. Add / View Transactions**
- The employee can record new sales transactions through the **Add Transaction** option.  
- The employee can view previous sales records by date or product through the **View Transactions** section.  
- The system saves new sales data and automatically updates stock quantities.  
- This enables accurate and efficient tracking of sales activities.  

---

#### **Employee Flow Overview**

![Employee Flowchart](assests/images/employee.svg){ width="20%" style="display:block; margin-left:auto; margin-right:auto;"}

## **System-Wide Functionalities**

| **Function** | **Description** |
|:--------------|:----------------|
| **User Authentication** | Validates user login credentials (owner or employee). |
| **Role-Based Access Control** | Determines actions based on the logged-in user’s role. |
| **Stock Updates** | Adjusts stock after each sale or inventory change. |

---


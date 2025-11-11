# **Functional Documentation**

## **Introduction**

This document outlines the **functional behavior** of the Inventory Management System (IMS) from the **end-user’s perspective**.  
It describes how users — **manager** and **employees** — interact with the system, what functionalities are available to them, and how the system responds to their actions.

The goal is to provide a clear understanding of the **system’s functionality**, ensuring that each feature aligns with user needs and business objectives.

---

## **Functional Requirements — manager**

#### **1. Login**
- The manager logs into the system using valid credentials.
- The manager enters their username and password, then clicks the **Login** button.
- The system Verifies credentials and grants access to the manager dashboard.  
- This ensures secure access to administrative functionalities.

---

#### **2. Manage Products**

- The manager can view, add, update, or delete products from the inventory.
- The manager navigates to the **Product** section to use options such as **Add Product**, **Edit**, or **Delete**
- The system adds, updates or deletes the product.
- This Provides full control over product inventory.

---

#### **3. Manage Transactions**
- The manager can record new transactions for purchases and can add new inventory.  
- The manager navigates to the **Transactions** section and selects **Add Transaction** to record data.  
- The system saves new transaction data and automatically updates stock quantities.  
- The manager can view previous transaction records in the **View Transactions** section.  
- This enables effective tracking of all business operations.  

---
#### **Onwer Flow Overview**

![Manager Flowchart](assests/images/manager.svg){ style="display:block; margin-left:auto; margin-right:auto;"}

## **Functional Requirements — Salesperson**

#### **1. Login**
- The salesperson logs into the system using valid credentials.  
- The salesperson enters their username and password, then clicks the **Login** button.  
- The system validates the credentials and grants access to the salesperson dashboard.  
- This ensures secure access control and prevents unauthorized usage.  

---

#### **2. View Products and Details**
- The salesperson can view all available products along with their details such as name, quantity, and price.  
- The salesperson navigates to the **Products** section to browse the available stock.  
- The system displays a list of products with their details but restricts editing or deletion.  
- This allows the salesperson to assist customers efficiently based on stock information.  

---

#### **3. Add / View Transactions**
- The salesperson can record new sales transactions through the **Add Transaction** option.  
- The salesperson can view previous sales records by date or product through the **View Transactions** section.  
- The system saves new sales data and automatically updates stock quantities.  
- This enables accurate and efficient tracking of sales activities.  

---

#### **salesperson Flow Overview**

![Salesperson Flowchart](assests/images/salesperson.svg){ width="20%" style="display:block; margin-left:auto; margin-right:auto;"}

## **System-Wide Functionalities**

| **Function** | **Description** |
|:--------------|:----------------|
| **User Authentication** | Validates user login credentials (manager or employee). |
| **Role-Based Access Control** | Determines actions based on the logged-in user’s role. |
| **Stock Updates** | Adjusts stock after each sale or inventory change. |

---


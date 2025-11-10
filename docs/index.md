# **Overview**

Welcome to the documentation of Inventory Management System.

## **Introduction**

The **Inventory Management System (IMS)** is designed to help mid-level shops and marts efficiently manage their inventory, sales, and keep track of their purchasing. These businesses are typically operated by an **owner** who supervises a few **employees or sales assistants**.  

This system aims to minimize manual errors and simplify day-to-day stock management for many **mid-sized retail stores** — such as various types of marts for shopping where inventory is still tracked manually leading to data inconsistency, delays, and mismanagement.

## **Objectives**

The primary objectives of the Inventory Management System are:

- **Efficient Stock Management**  
  To provide a platform where admins can add, update, or delete product information and track stock quantities.
- **Role-Based Control**  
  To ensure that access privileges are granted according to user roles (Admin or employee).
- **Transaction Tracking**  
  To maintain a record of all sales and purchase transactions.
- **Improved Visibility**  
  To allow visibility of all the products available, making it easier for the employee to interact with customers.
- **Error Reduction**  
  To minimize manual entry errors and duplication by automating stock updates after each transaction.


## **Tech Stack**

| Category             | Technology / Tool        |
|----------------------|--------------------------|
| Backend Framework | Django REST Framework     |
| Frontend          | HTML, CSS, JavaScript     |
| Database         | PostgreSQL       |
| Mobile Application | PWA                 |
| Documentation     | MkDocs                   |

## **User Roles and Permissions**

| Role          | Permissions / Capabilities |
|----------------|-----------------------------|
| Admin (Owner) | - Add, edit, or delete products.<br>- Update stock quantities.<br>- Record transactions (sales or purchases).<br>- View all transactions (own and employees’).|
| employee | - View available products and their quantities.<br>- Record sales transactions only.<br>- View only their own transaction history. |

## **Future Scope**

- The owner will be able to view last month's purchase and sales visualization in dashboard. 
- The employee will be able to add invoice along with transactions.
- Automated low stock alerts.
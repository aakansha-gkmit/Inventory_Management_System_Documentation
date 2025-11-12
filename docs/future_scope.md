# **Future Scope**

The Inventory Management System (IMS) in its current version provides a solid foundation for managing products, transactions, and user roles. However, several enhancements are planned to further expand its analytical capabilities, operational efficiency, and business intelligence.

## **Dashboard Enhancements and Analytics**
Future updates will introduce advanced visual analytics for the admin dashboard. Administrators will be able to view detailed visualizations of purchase and sales data from the previous month, including interactive graphs and trend summaries. These insights will enable better performance monitoring and strategic decision-making. Over time, additional filtering and comparative visualization features may also be integrated to allow detailed exploration by date range, product category, or employee activity.

## **Automated Stock Management**
The system will include automated low-stock alerts to notify administrators when product quantities drop below a defined threshold. This feature will support proactive restocking and prevent stockouts that may affect sales continuity. Alerts may later be extended to include supplier integration for faster replenishment.

## **Customer Management Integration**
Currently, the system does not maintain customer information. A dedicated customer module will be introduced to store and manage customer details. This addition will enable the system to generate customer-specific sales reports, track purchase histories, and support loyalty or promotional initiatives in the future. Maintaining customer data will also improve overall business intelligence by providing deeper insights into customer behavior and sales trends.

## **Cost Price and Profit Analysis**
At present, the system focuses on tracking only the selling price of products. Future versions will include cost price management to facilitate accurate profit margin analysis. This enhancement will enable the calculation of profit and loss reports, helping administrators understand product-level profitability and make informed pricing decisions. Because both cost and selling prices may change over time, the system will maintain historical pricing records to ensure the accuracy of financial analyses.

---

# **Future Schema Diagram**

![Future Schema Diagram](assests/images/future_data_model.svg){ width="180%" style="display:block; margin-left:auto; margin-right:auto;"}

## Future Scope: Enhanced Data Model and Normalization

The enhanced Entity-Relationship Diagram (ERD) represents a forward-looking expansion of the existing system’s data architecture. While the core modules—**Users**, **Products**, and **Transactions**—form the foundation of the currently implemented system, the updated model introduces several additional entities and relational refinements to support future growth and functionality.

One of the key enhancements involves restructuring the **role management** mechanism. In the earlier version, user roles such as *Admin*, *Manager*, and *Salesperson* were defined using an enum field within the `USERS` table. Although this approach was effective for initial implementation, it limited flexibility for role updates or expansions. The new design replaces the enum with a dedicated `ROLES` table and a junction table `USER_ROLES`, enabling a many-to-many relationship between users and roles. This allows for dynamic role assignment and easier introduction of new user roles without altering the database schema.

Another major improvement is the **replacement of enum fields for product categories and transaction types** with separate relational tables—`CATEGORIES` and `TRANSACTION_TYPES`. Previously, these attributes were stored as enums, making it difficult to extend or describe them in more detail. By modeling them as individual entities, the database achieves higher normalization and flexibility. Each product now references a single category, and each transaction references one type, maintaining one-to-many relationships without requiring additional junction tables. 

The introduction of **customer and invoice management** marks another significant step in system evolution. The new `CUSTOMERS` table allows storage of customer information such as name, contact details, and address. The `INVOICE` table links each transaction to a specific customer, including billing details, payment method, and due dates. This enhancement transitions the system from a basic inventory and transaction tracker into a more comprehensive business management solution, capable of generating and maintaining sales documentation for real-world use cases..

Overall, these updates are positioned within the **future scope** of the project. The existing implementation already supports key functions such as authentication, authorization, inventory tracking, and transaction recording. The proposed enhancements, however, aim to future-proof the system by enabling multi-role management, customer integration, flexible categorization, and structured invoicing. 

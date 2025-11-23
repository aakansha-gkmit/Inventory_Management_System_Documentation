<!-- # **Frontend Testing Plan**

## **1. Login**
**Objective:** Ensure secure and accurate login functionality for all users.

#### **Testing Focus:**
- Valid credentials should redirect users to their respective dashboards (Manager or Salesperson).  
- Invalid credentials should display a clear “Invalid credentials” error message.  
- Empty username or password fields should trigger a “Please enter username and password” prompt.  
- Password visibility toggles should work correctly.  
- Login form layout and elements should be responsive across devices.  
- Role-based redirection must be verified: Managers see the Manager Dashboard, Salespersons see the Sales Dashboard.  

---

## **2. Product Listing**
**Objective:** Validate correct display of product information with search and filter functionalities.

#### **Testing Focus:**
- All products should be listed with essential information such as name, price, and stock availability.  
- Managers should see full product details, including stock levels; Salespersons see limited details.  
- Search and filter functions should return accurate results.  
- If no products are available, an informative message like “No products available” should be displayed. 

---

## **3. Add Inventory (Manager Only)**
**Objective:** Ensure managers can manage inventory effectively.

#### **Testing Focus:**
- Mandatory fields such as product name, price, and quantity must be validated.  
- Numeric fields should reject non-numeric input.  
- Successful product additions should appear in the product listing.  
- Only Managers should have access to this functionality; it must be hidden from Salespersons.  

---

## **4. Sales Transaction**
**Objective:** Confirm accurate processing of sales transactions and stock management.

#### **Testing Focus:**
- Salespersons can select products, enter quantities, and complete transactions.  
- Stock limits are enforced; attempting to sell more than available stock should display an error.  
- Total price calculation should be accurate (product price × quantity).  
- Role restrictions must be enforced: Managers may view transactions but cannot create sales; Salespersons cannot access inventory management.  
- Successful transactions should generate confirmation messages.  

---

## **5. View Previous Transactions**
**Objective:** Provide accurate visibility of historical sales records.

#### **Testing Focus:**
- Transaction history should display relevant details such as product, quantity, price, and date.  
- Managers can view all transactions; Salespersons can view only their own transactions.  
- Display a message like “No transactions found” if there are no records. 

--- -->

# **Backend Testing Plan** 

## **1. Authentication**
**Objective:** Ensure secure and reliable user authentication.

#### **Testing Focus:**
- Users can register or login with valid credentials.  
- Invalid credentials should return proper error messages without exposing sensitive information.  
- JWT tokens are generated correctly and include user role information.  
- Token expiration is enforced, and refresh tokens work as expected.  
- Passwords are securely hashed before storing in the database.  

---

## **2. Role-Based Access Control**
**Objective:** Enforce access restrictions according to user roles (Manager, Salesperson).

#### **Testing Focus:**
- Managers can perform all inventory-related actions (add, update, delete products).  
- Salespersons can only perform sales transactions and view relevant data.  
- Unauthorized role access should return appropriate error messages.  
- API responses respect role-based filters, e.g., Salespersons see only their transactions.  

---

## **3. Product Management**
**Objective:** Validate correct creation, update, retrieval, and deletion of product data.

#### **Testing Focus:**
- API endpoints correctly handle creating new products (Manager only).  
- Product updates reflect accurately in the database.  
- Deleting products removes the correct entry or marks it as inactive if soft delete is implemented.  
- Fetching product lists returns accurate data, including stock levels and price.  
- Edge cases like duplicate product names or invalid input types are handled gracefully.  

---

## **4. Sales Transactions**
**Objective:** Ensure accurate recording and processing of sales.

#### **Testing Focus:**
- Transactions can be created only with valid product IDs and available stock.  
- Total amount is calculated correctly on the backend.  
- Stock is updated appropriately after each transaction.  
- Attempting a transaction with insufficient stock should return a clear error.  
- Salespersons can view only their transactions; Managers can view all.  
- Transaction history endpoints support filtering by date, product, and user.  

---

## **5. Data Validation and Error Handling**
**Objective:** Ensure backend handles invalid or unexpected inputs properly.

#### **Testing Focus:**
- All input fields are validated for correct types and required constraints.  
- Invalid data returns meaningful error messages.  
- API endpoints handle missing, malformed, or extra parameters.  
- Edge cases (e.g., extremely large numbers, special characters) are handled safely.  

---



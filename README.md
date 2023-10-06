# DemoMarketPlace-Project-Solution
# Demo Marketplace Python Project Documentation

The Demo Marketplace is a Python project that simulates a simple marketplace where users can browse products, add them to their cart, and place orders. The project provides functionality for both regular users and administrators. Users can create accounts, log in, view the product catalog, add products to their cart, remove products from the cart, view their cart, and place orders. Administrators have additional privileges such as add/edit product or category

## Functionality

The Demo Marketplace project provides the following functionality:

### 1. Display a Welcome Message

The `display_welcome_message()` function displays a welcome message when the program starts.

### 2. Create Admin

The `create_admin(username)` function allows you to create an administrator account. Administrators have additional privileges compared to regular users.

### 3. Create User

The `create_user(username)` function allows you to create a regular user account.

### 4. Create Sample Products

The `create_sample_products()` function creates some sample products and adds them to the product catalog. Each product has a unique product ID, name, category, and price.

### 5. Login

The `login(username)` function allows users and administrators to log in to their accounts. After logging in, the current user is stored in the `current_user` variable, which is used for performing user-specific actions

### 6. Logout

The `logout()` function logs out the current user by setting the `current_user` variable to `None`.

### 7. View Catalog

The `view_catalog()` function displays the product catalog. It lists the product ID, name, category, and price of each product.

### 8. Add to Cart

The `add_to_cart(product_id, quantity)` function allows the current user to add a product to their cart. The function checks if the user is logged in and if the product ID is valid before adding the product to the cart.

### 9. Remove from Cart

The `remove_from_cart(product_id)` function allows the current user to remove a product from their cart. The function checks if the user is logged in and removes the product from the cart if it exists.

### 10. View Cart

The `view_cart()` function displays the contents of the current user's cart. It lists the products in the cart along with their quantities and calculates the total price of the cart.

### 11. Checkout

The `checkout(payment_method)` function allows the current user to place an order and complete the checkout process. The function checks if the user is logged in, if the cart is empty, and if the payment method is valid. If the payment method is valid, it simulates a payment process by generating a random transaction ID.

- [ ]  **User Authentication:**

Test **user** login with an invalid username. Test **admin** login with invalid username

**Data Validation:**

Validate that the application properly handles invalid **data** inputs and **provides appropriate error messages**.

**Product Catalog:**

Verify that the **product** catalog is displayed correctly. Check if users can see product details such as name, category, and price. Verify that the admin can see the **product catalog**.

**User Cart:**

Add items to the user's **cart**. Remove items from the user's cart. **Verify** that the cart contents are displayed correctly. Ensure that users cannot access admin-specific cart functions.

**Admin Product Management:**

Add a new **category** to the catalog as an admin. Ensure that users cannot access admin-specific product management functions.

**Session Management:**

Test user session management **(login, logout)**. Test admin session management (login, logout). Check if users and admins are redirected to the login page when not authenticated. Verify that error messages are displayed when appropriate.

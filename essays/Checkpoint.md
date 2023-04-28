---
layout: essay
type: essay
title: "Checkpoint Assignment #3"
# All dates must be YYYY-MM-DD format!
date: 2023-04-27
published: true
labels:
  - MIS
  - Checkpoint
  - Assignment 3
---

1. Link to my screencast [here](https://youtu.be/EgVxgw8ezFo)

Site Map
![sitema](https://github.com/bctrxn/bctrxn.github.io/blob/main/site_map.jpeg)

2. Describe your design for your site’s shopping cart. That is, will it be a separate page that the user can view and edit, or will it be integrated into the product pages? If so, describe in detail how this will work on your site. Provide several examples of using the cart.
My shopping cart will be a separate file that displays the user’s session information. Users can access the cart at any time and they can also update the cart from the cart page without having to go back to the products display page. When users click complete purchase on the cart page, they will be redirected to the invoice.

3. Explain specifically how you will use sessions to manage your shopping cart. In particular, what shopping cart data will be stored in the session, what data format will be used (NOT what data type, but the format like with the data format used for your registration data). Use code examples showing what data structures (such as arrays and their objects) you will use to manage the shopping cart data and how they will be used in a session.
I will store the user’s selected quantities in the session and will use that to display their cart information, as well as to make values in input boxes sticky. 
     -  The session will be managed on the server side and sent to the client side whenever a request for the cart is made.
     -  I will store the different product categories in the cart as arrays and the values within those arrays will be the values that the user selected.
     -  Every time the user adds another product to their cart, the quantity they selected will be pushed to the array.

4. How will you avoid access to your application when the user has not logged in or registered? What are the particular security concerns you must address?
I will address login security concerns using cookies. When the user logs in, i will give them a cookie that verifies that they have entered the appropriate credentials and are able to complete the purchase. If a user does not have a cookie, I will send them to the login page when they try to proceed to the invoice. Each cookie will last 15 minutes. After 15 minutes is up, the user will be logged out and will have to log back in again if they wish to complete their purchase.

5. Upon a successful login, how do you provide personalization in your UI? Explain how you did or will do this (paste code if necessary)
Upon successful login, I will change the login button on the nav bar to display the user’s name. I will also add welcome messages to the home and invoice pages. I will also make it so the total number of items in the user’s cart is displayed on the nav bar.

6. If you are working with partners, how will you split up the work in your team so that you are working in parallel as effectively as possible? That is, who is doing what and when?
I am not working with a partner.

7. How are you approaching Assignment 3 differently than Assignment 2?
I used the same files as assignment 2. However, I had to adjust the for loops to take into account the three different categories of products and I also had to re-route the path of my site. This is because the user can now log in at any time and they can also add and remove items from the cart without needing to log in. 

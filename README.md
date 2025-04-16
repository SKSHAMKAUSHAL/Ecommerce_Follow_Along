'E-commerce website' follow along project for Semester 2

Milestone 1: Project Overview

In todays live session our mentor introduced us to overall structure of MERN Stack. He taught us the foundational steps to set up the environment for future milestones, we created a new repository for our follow along project.

Milestone 2: Front-end setup and login page

In todays live session we learnt to organize the files into separate frontend and backend directories.

Set up React for frontend

Node.js setup for backend

Tailwind CSS configurations

We also designed the front end for login page of the e-commerce application.

Milestone 3: File organizing and MongoDB

Set up dedicated folders for organizing backend code effectively. Initialize and configure a Node.js server to handle API requests. Connect your application to MongoDB to store and manage data. Implement basic error handling to ensure your server runs smoothly.

Milestone 4: Created and Configured Files

Created a User Model: Our mentor explained how a MODEL in MVC architecture works and how it interacts with database. Created a User Controller: We got to know the purpose of a controller in MVC. Enable and Configure Multer: In the live session mentor told us what is a multer and what is it used for and how it can be configured to handle file uploads.

Milestone 5: Created Frontend UI for signup page and added the code for authentication of the inputs

In this part of the Follow Along project we made the UI (Frontend) for the sign up page of our website. This page allows the users to add their details.

After the user is done with entering backend comes into play. Backend does the form validation part, it verifies whether the user has entered the details in the right format(e.g. email, minimum length)

Milestone 6:

Encrypt the Password Using bcrypt
During the user signup process, encrypt the user's password using the bcrypt hashing algorithm. This ensures that the password is stored in a secure, non-reversible format. The bcrypt algorithm adds a "salt" to the password before hashing, making it resistant to common password-cracking techniques. The hashed password should never be stored in plain text.

Save the Hashed Password in the Database
Only store the hashed version of the password in the database. Do not store plain text passwords for security reasons. Ensure the hashed password is securely saved in the database along with other user information.

Store Complete User Data
In addition to the hashed password, save the user's other information, such as their name, email, and any other relevant data. The complete user data should be stored securely, ensuring that sensitive information like the password remains encrypted.

Handle Login with Hashed Passwords
During the login process, compare the entered password with the hashed version stored in the database. Use bcrypt to safely verify if the entered password matches the stored hash.

Milestone 7

Create Login Endpoint: Accept user credentials (email/username and password). Retrieve the corresponding user from the database.

Validate Password: Use bcrypt to hash the entered password. Compare it with the stored hashed password for authentication.

Milestone 8

Create the Card Component:
Design a reusable card component with props for product details (e.g., name, image, price).

Design the Homepage Layout:
Set up a grid layout or flexbox for displaying multiple cards neatly.

Milestone 9

Create the form for products

This form will take multiple product images images as input

Milestone 10

Define the structure of product data (e.g., name, description, price, image URL) using Mongoose. -Ensure each field has proper validation (e.g., required fields, correct data types).

Build a POST endpoint to receive product data.

Validate and save the product details to MongoDB.

Milestone 11

Write an endpoint that will send all products data to frontend In frontend write an function to get all the data Display these data dynamically passing to product card component.
Milestone 12

Write an endpoint that will send all products with user mail to frontend In frontend write an function to get all the data Display these data dynamically passing to product card component.
Milestone 13

Write an endpoint that will receive new data and update the existing data inside MondoDB. In frontend we will add an edit button to the product card. When click on edit we will send the data to form and make it auto fill and have option to edit those data and save.
Milestone 14

1.Write an endpoint that will Delete the data form MongoDB using ID. In frontend we will add an delete button to the product card. When click on delete button we will send the product id to server endpoint.

milestone 15  

Create an new Nav component with links to all pages:

Home
My-products
Add product
cart
Make the Navbar responsive to all screen sizes.

We will add the nav component to all the pages and make the navigations to all this pages smooth and easy.


milestone 16--->

Create an new page that display all the product data


milestone 17 -->

Write the cart schema to store products
Write an endpoint to store receive and store product details in cart





 Milestone 18  ---->
Create an Backend endpoint for cart page
Write and endpoint to get products inside cart for user


MILESTONE 19 --->

create cart frontend page and display the products
For each product add an option to increase and decrease quantity using + and - buttons.
Create an Backend endpoint for increase and decrease quantity



 Milestone 20📝--->
Create an Backend endpoint that will sent user data
create frontend profile page
display profile photo, name and email in one section
In another section display address and add an button called "Add address"
If there are no address display "No address found"



Milestone 21📝
create address form frontend page
Create an state that will store input address
when we click on add address in profile it should navigate to this form page.



Milestone 22📝
You need to create an endpoint that will receive the address from address form in frontend
Add the address to the address array inside user collection.


Milestone 23📝
Create an placeorder button inside cart page and navigate to select address page when clicked.
Create and select address page that will display all the available address and have an option to select one address.
Write an backend endpoint that will send all the addresses of the user.



Milestone 24📝
First we will display all the products we are ordering
Next we will display the address user selected to deliver
We will display the total value of the cart
We will have an place order button at the bottom.


Milestone 25📝
You need to create an endpoint that will receive the products, user, address details
You will get the mail of the user using that you need to retrive the _id of the user
For each product the order will be different with same address
using order schema you created earlier you will store order details in mongodb order collection


 Milestone 26📝
You need to create an endpoint that will receive the user mail
You will get the mail of the user using that you need to retrive the _id of the user
Using that _id you need to get all the orders of that user
Send all the users orders in the response.






Milestone 27📝
You need to create an my-orders page
You will send an get request to my-orders endpoint that we created in previous milestone.
We will send user mail in to endpoint to get all the user orders
Display all the user orders
We will add my-orders page in navbar for better navigation.


Steps for Milestone 28📝
In my-orders page for every order add cancel order button
If the order is already canceled this button should not be displayed
You need to create an endpoint that will receive the order-id
Get the order using this id and mark the status canceled and save


Steps for Milestone 29📝
Please create an PayPal account first PayPal developer dashboard
Once you login you can see an option for an sandbox accounts.
Copy the UserID of that account and save it.
In this sandbox accounts you can find your client id copy and save it.
In your order conformation page you need two options for payment one is COD and another is online payment.
Create radio buttons to select COD or online payment and when we click on online payment PayPal buttons need to be displayed.
In next milestone we will write an code to display and use those PayPal online Payments buttons.



Steps for Milestone 30📝
After creating PayPal account and getting the UserID inside sandbox account.
Implement online payment using PayPal API using the client key you created earlier.
Download NPM package called react-paypal-js that will provide an component called PayPalScriptProvider which will display online payment methods like credit or debit card etc..,
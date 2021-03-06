# Student-Marketplace
Final assignment for McGill Comp 307 - Introduction to Web development. A marketplace web app built using React and Django. 

## Authors
Zachary Probst, Steven Shao and Trisha Winterson Chagnon



## Set up Instructions


1.    Frontend (react)

a.     Install node.js (> 12.16.1) , npm (> 6.13.4)

b.   install dependencies in Frontend/gui-react/package.json using npm install 

c.   run frontend application on localhost:3000 using npm start (in gui-react folder)

2.    Backend

a.    Assume already installed: python3, redis, pip3

b.    Install dependencies: (we have included venv, so please try skipping this step)

                                      i.     Cd to /Backend (then the following in terminal)

                                    ii.     python3 -m venv venv

                                   iii.     source venv/bin/activate

                                   iv.     pip3 install requirements.txt

c.     To run (in terminal):

                                      i.     redis-server

                                    ii.     python3 manage.py runserver

3.    Login:

a.    Because mailgun is configured to our emails, you cannot register properly. Please email me (steven.shao@mail.mcgill.ca) so I can add you to mailgun.

b.    You can login to our app with existing user:

                                      i.     Username: steven.shao@mail.mcgill.ca

                                    ii.     Password: password


## Design Doc

### Business Problem
Universities do not have online marketplaces for students to <u>easily
and securely</u> buy, sell and exchange items.

### Use Cases (Requirements)
1.  As a student, I would like to buy, sell and exchange items within my
    university.
2.  As a buyer, I would like to see a list of all items for sale.
3.  As a buyer, I would like to add items to cart and checkout online.
4.  As a buyer, I would like to see my purchase history.
5.  As a student, I would like to chat with other students.
6.  As a seller, I would like to add, modify or remove product listings,
    and see all of my listings.

### Features (Matching Requirements)
1.  <u>Registration page</u> Email validation during
    registration using MailGun.
2.  <u>Product listing page</u> showing all items for sale. Users
    can add items to cart.
3.  <u>Cart page</u> showing total price. Users can checkout
    using PayPal or Stripe.
4.  <u>Purchase history page</u> showing purchases.
5.  <u>Chat page</u> for each user. Other users can join and
    leave messages. (In my opinion this is easier to implement for the
    frontend because we don't need different tabs for chats with
    different users).
6.  <u>Control panel page</u> that allows users to list products
    to sell (add, update and delete). All products belonging to the user
    are shown on this page.

### UI
1.  Login page
2.  Registration Page
3.  Product listing page
4.  Cart page
5.  Purchase history page
6.  Chat page
7.  Control panel page

### Milestones
1. Research phase
  - Date: February 13, 2020
  - Steven: setting up Django backend, account management, product picture
  - Trisha: Google Maps API, chat/websocket
  - Zach: UI, Cart feature cache

See Word doc under Documentation for more details.

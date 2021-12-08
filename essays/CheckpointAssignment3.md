---
layout: essay
type: essay
title: Check Point for Assignment 3
# All dates must be YYYY-MM-DD format!
date: 2021-12-07
labels:
  - Checkpoint
---


# Shopping Cart Design
The shopping cart will hold items that the guests select. It should be visible on products_display and login page. The guests will be able to view and edit. It will ask to loggin if they want to store items in cart. It will save on the memory of the session. It should store username to the cart.


# Use code examples showing what data structures (such as arrays and their objects).
you will use to manage the shopping cart data and how they will be used in a session.

app.get("/add_to_cart", function (request, response) {
    var products_key = request.query['products_key']; 
    var quantities = request.query['quantities'].map(Number);
    request.session.cart[products_key] = quantities;  
    response.redirect('./cart.html');
});
    I will try to use example codes. This will allow me to get the product key from post and get qutntities, convert strings to numbers and store in array
    
# How will you avoid access to your application when the user has not logged in or registered? What are the particular security concerns you must address?
I will send them back to login page if they are not logged in. If they are not registered they should sign up first.

# how do you provide personalization in your UI? Explain how you did or will do this (paste code if necessary)
New users need to register in order to place an order. If everything mathes they will be sent to cart or invoice otherwise sign up page.

# How are you approaching Assignment 3 differently than Assignment 2?
I am still not confident with coding. I will try to learn from examples and look up on google for documentations and youtube videos for further explanations. I will meet more often with professor to get a better idea.

https://hawaii0-my.sharepoint.com/:p:/g/personal/yejinj_hawaii_edu/EbpW710ximxPh6iORDgv_90BxDF7fGOoPvV83YY_qg9Dug?e=MbsHcd

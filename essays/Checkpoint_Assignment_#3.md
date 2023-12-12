
---
layout: essay
type: essay
title: "Checkpoint Assignment #3"
# All dates must be YYYY-MM-DD format!
date: 2023-12-11
published: true
labels:
  - Essay
  - Assignment3
  - Checkpoint Assignment #3
  - Group
---

## Show what each page will look like. The pages do not have to be “functional” but the design should be clear. Here is an example PPT prototype


Click HERE [link](https://dport96.github.io/ITM352/morea/150.Assignment2/experience-Assignment2_retrospective.html) for a brief overview of our prototype layout and functionality for our Assignment 3 e-commerce website.

<img width="500px" src="../img/A3 map.png" />

## 1. Describe your design for your site’s shopping cart. That is, will it be a separate page that the user can view and edit, or will it be integrated into the product pages? If so, describe in detail how this will work on your site. Provide several examples of using the cart.

Our design includes a dedicated shopping cart page, where users can manage the quantities of their chosen products. This page will bear a resemblance to the invoice page, offering a preview of selected items and their quantities for final confirmation. The cart functionality hinges on session-based data storage, maintaining the user's selection details. Users have the flexibility to modify product quantities directly in the cart, either by increasing or deleting them entirely. Once satisfied with their choices, they can initiate the purchase process by clicking the "Complete Purchase" button, leading them to the Invoice page. However, access to the invoice page requires either logging in or registering an account. Unauthenticated users will be redirected to the login page to ensure secure processing.

## 2. Explain specifically how you will use sessions to manage your shopping cart. In particular, what shopping cart data will be stored in the session, what data format will be used (NOT what data type, but the format like with the data format used for your registration data). Use code examples showing what data structures (such as arrays and their objects) you will use to manage the shopping cart data and how they will be used in a session.

Our strategy involves leveraging session management to handle the data in our shopping cart, particularly focusing on the quantities of products inputted by users. Each product type will be represented as a key, with its corresponding quantities stored in an array format within the shopping cart. For example, if a user selects products across various pages, the data structure in the cart would resemble an array like this: {Gellie: [1, 2, 3], Nerissa: [4, 5, 6]}. This approach ensures an organized and accessible way to track and manage product selections.

## 3. Explain specifically how you will use sessions to manage your shopping cart. In particular, what shopping cart data will be stored in the session, what data format will be used (NOT what data type, but the format like with the data format used for your registration data). Use code examples showing what data structures (such as arrays and their objects) you will use to manage the shopping cart data and how they will be used in a session.

To enhance the security of my application and safeguard against unauthorized access, I plan to implement a robust authentication system using cookies. This approach will be particularly critical during the shopping process. When a user attempts to make a purchase, the server will check for the presence of a valid cookie to confirm that the user is currently logged in. If the user's session is authenticated via the cookie, they will be smoothly directed to the invoice page to complete their transaction. Conversely, if a user does not have a valid cookie, indicating they are not logged in, they will be redirected to the login page where they can either sign in or register a new account.

I'm aware of the potential vulnerabilities associated with using cookies, such as the risk of unauthorized access or tampering. To mitigate these risks, I intend to implement enhanced security measures, like using secure and HttpOnly flags on cookies, and possibly integrating additional safeguards such as encryption and regular cookie validation checks. This multi-layered approach aims to ensure a secure and user-friendly experience, maintaining both the integrity and confidentiality of user data.

## 4. How will you avoid access to your application when the user has not logged in or registered? What are the particular security concerns you must address?

Addressing security concerns is paramount in ensuring that users cannot access each other's data. A key strategy to achieve this is through the use of cookies, which play a crucial role in session management. Hence, our website mandates users to log in or register before finalizing their purchases, even though they can freely edit their shopping carts. The use of cookies is instrumental here; they enable us to maintain a user's login status temporarily, confined to the duration of their active session.

However, it's important to acknowledge that cookies, residing on the client side, are not completely foolproof and are susceptible to manipulation. Therefore, while using cookies to verify a user’s status is generally effective, it's not an all-encompassing solution. To bolster security further, I plan to implement a session timeout feature. This means if a user remains inactive for a predetermined period, the website will automatically terminate their session and log them out. This additional measure significantly reduces the risk of unauthorized access, ensuring that user data remains secure and private.

## 5. Upon a successful login, how do you provide personalization in your UI? Explain how you did or will do this (paste code if necessary)

Assignment 2 posed greater complexity, particularly concerning the login and registration pages, including the incorporation of IRs. Handling data within the user JSON file was a significant aspect involving code retrieving existing data and updating it with new registration information. Although more extensive, this assignment improved my overall comprehension.

## 6. If you are working with partners, how will you split up the work in your team so that you are working in parallel as effectively as possible? That is, who is doing what and when?

Absolutely, teaming up with partners is a big part of what we're doing. We're all about working together in sync, tackling one thing at a time. This way, we really get what each other is thinking and doing. It's all about making things smoother and quicker, especially when it comes to fitting our code pieces together.

We're putting all our brains on one task instead of spreading thin over many. That way, we get stuff done better and faster. Plus, we're big on keeping in touch. If any of us figures out something cool or important on our own, we'll make sure to fill in the others right away. This keeps us all in the loop and makes it easy to pick up where someone else left off, keeping our teamwork tight and on point.

## 7. How are you approaching Assignment 3 differently than Assignment 2?

Assignment 3 presents a unique set of challenges, potentially even more complex than those of Assignment 2. I'm currently evaluating whether I need to start anew. A key aspect that sets Assignment 3 apart is the emphasis on user experience in my coding process. It's crucial for me to ensure that users can easily navigate through all the web pages while maintaining the security of their data.

This task involves implementing numerous validations and making significant user interface adjustments. Additionally, I need to be mindful of the user's journey throughout the website, tracking their movements across different pages. That's why having a detailed outline is invaluable – it helps me to visualize and plan the user's navigation path on my website, aiming for a seamless and intuitive experience.

---
layout: project
type: project
image: img/Weniled2.png
title: "Assignment 2"
date: 2023
published: true
labels:
  - Final Assignments
  - Assignment 2
  - Reflection/Review
summary: "In Assignment 2, we were tasked with improving Assignment 1's personalization and security. This involved creating a registration and login system where users could save their data, making it persistent. The website was tailored to greet users by name post-login and use their names in invoices. Only registered users were allowed to make purchases, though product viewing was unrestricted. Key requirements included multiple-user support, secure login verification, and a personalized user experience. Additional goals were to improve the user interface, code readability, and overall program design. The project emphasized server-side validation, avoiding sessions or cookies, and focused on user case scenarios in design and implementation."
---

In Assignment 2, we had to work off our Assignment 1 to make our e-commerce page more secure and personalized. In Assignment 2, we were tasked with making sure that we add securtiy features in our shop. Instead of just being able to buy products and get redirected to an invoice. Users are no longer able to do so, without having an account. When they try to proceed and buy the products they will be immedictaely redirected to a login-page. Users will have to create an account or log in with their account. The login shows users how many other active users are on the shop as well and a toggle feature for friendly user experience. The create an account page has users enter their name and email as well, as a secured password. If the password doesn't meet all certain secruity measures, the system will not allow them to succesfully regster their account. It also tells the users what's wrong with their account if there is an error. I also implemented a  I implemented all the individual requirements for extra credit, earning the highest grade in the class and standing out as a unique and innovative e-commerce concept.

## Individual Requirements   
-**IR1** Store passwords encrypted. When the user registers, encrypt their password before saving the registration data to the file. When a user logs in, encrypt the password they entered and compare it with the encrypted saved password. Do not decrypt the password. You may find the crypto library useful.

-**IR2** Require that passwords have at least one number and one special character.

-**IR3** When the user is registering, suggest a “strong” password that is 10 random characters including numbers and special characters.

-**IR4** Keep track of the number of times a user logged in and the last time they logged in. When they login display this information.

-**IR5** Keep track of the number of users currently logged in to the site and display this number with the personalization information. For example, if user “dport” is logged in and there are 4 other users logged in, then each page should say somewhere “Welcome Dan, there are 4 users currently using this system.” Whenever a user logs out (for this assignment, put a logout button on the invoice page that removes the login identification and sends the user to the login page), the number should decrease accordingly. HINT: Store this information as a global array variable on the server. Whenever a user logs in or registers, add their email address (or username) to the array.

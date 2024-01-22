---
layout: project
type: project
image: ![WeNailed Logo](img/WeNailed_optimized.png)
title: "Assignment 1"
date: 2023
published: true
labels:
  - Final Assignments
  - Assignment 1
  - Reflection/Review
summary: "Assignment 1 tasks students with creating an e-commerce website selling products or services of our choice. They must enable users to select quantities, validate input, calculate totals with tax and shipping, and display invoices. The project covers building an information system, designing a user interface, processing input on a server, and using dynamic data sources. Students use arrays of objects for product display, implement server-side data validation, and ensure good UI design. This assignment is part of a larger 3-part project, serving as a foundational step for our final assignments."
---

In Assignment 1, I developed an e-commerce website named "Wenailed" specializing in press-on nails. I devoted significant effort to ensuring robust server-side data validation and an appealing UI design. Going beyond the basic requirements, I added an extra index page redirecting users to the homepage when they click the logo. The homepage seamlessly leads to a user-friendly interface resembling a real online shop catalog, featuring a popular holiday collection. A navigation menu lets customers explore different sections like contact, about, or shop pages. Users can use the navigation menu above or the "Shop Here" button on the homepage to access the shop page. For data validation, the system provides clear feedback to users when they input invalid quantities, explaining the issue and prompting corrections. It also prevents orders from exceeding available product quantities. Upon entering valid data, customers receive a thank-you invoice, with product descriptions displayed when hovering over product images. I implemented all the individual requirements for extra credit, earning the highest grade in the class and standing out as a unique and innovative e-commerce concept.

## Individual Requirements   
-**IR1** Track the total quantity of each item sold. This needs to be implemented on the server when you remove sold items from the quantity available. Display total quantity sold with the product information. Extra credit: have this dynamically update on the client when there are any purchases processed on the server (from other users).

-**IR2** Check that a quantity entered is valid (see three conditions given in the instructions above). If not, change the frame for the textbox to red and display a message with what’s wrong near the input e.g. “Quantity must be a number!”. If the input is valid, indicate this with a message “You want:”. Do not add a guard or HTML validation that would prevent the user from entering an invalid quantity. You do not need to do this on the server. But consider the quantity available when there are multiple users purchasing.

-**IR3** Check that the quantity entered does not exceed the quantity available as currently available on the server. If it does, change the frame for the textbox to red and display a message “We don’t have xx available.” and reduce the input to the quantity available (replace the input). The primary intent of this requirement is to let the user know that the amount they wanted when they try to purchase was no longer available if another user purchased before them. This means you must do this in a response from the server since it is the only place that has the current number available (consider the quantity available when there are multiple users purchasing). You do not need to do this on the server in response to a purchase, but this is probably the more straightforward way. If you only check the quantity available on the current page when the user enters it in the textbox, it will not prevent the quantity being unavailable on the server due to another users purchase. Extra credit: check if the quantity is available on the server and update the quantity available as the user enters the quantity in the textbox. That is, not in response to a purchase.

-**IR4** If the purchase is invalid (see three conditions given in the instructions above), change the purchase button text from “Purchase” to text that indicates why the purchase is invalid e.g. “Please Select Some Items to Purchase”. Do not disable the button or add a guard that prevents the user form purchasing.

-**IR5** When displaying the invoice, add a small icon image of the product to the line item. If the user hovers over the icon, have a popup window appear with a product description.

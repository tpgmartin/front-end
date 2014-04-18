OpenTable Front End Coding Challenge
=========

To start this project:
```
$ npm install
$ node app.js
```
Current project state
---
  - Reads in a json file that contains the restaurant and menu information.
  - Displays the restaurant name and the items in each section of the menu
  - Clicking on a menu item maintains a running total price in "Total"

Augmentations
---
Menu
  - style the menu so that it looks like menu-mock.png
  - display the description of menu items when they exist
  
Make a better display for "My Order"
  - show what dishes have been ordered so far
  - show a count for how many of each dish has been ordered
  - include 8% tax in the total
  - allow the person to select a tip percentage between [0, 5%, 10%, 15%, 20%], calculated on the pre-tax total
  
Some menu items are limited in quantity
 - for items with a limited quantity, add the word "special" to the end of the description of the item
 - display the remaining dish count if the count is less than 2
 - if the dish is sold out, change the font color of the text on the item to #aaa and ensure a customer cannot order it
 - Maintain the state of limited items once the customer pays (ie: when you refresh the page, the limited items reflect whether or not the items have been previously ordered)
 
create a "restaurant owner view" at /owner.  Don't worry about user validation.  The owner should be able to
 - add and remove items for any menu section
 - see the current count of all items and allow them to change the quantities
 - reorder the items in each section
 - when the owner saves the restaurant details, write the changes to the file
 
Feel free to
 - use any javascript libraries or css frameworks you wish.
 - add any node modules or middleware to app.js 
 - make it pretty in a mobile or desktop size
 - make it production ready
 - change/add/remove any folders or files
 - scrap this entire project and program the augmentations using the tooling/framework/language of your choice

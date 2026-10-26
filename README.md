# CS 360 Mobile Inventory App

## Project Summary

The application I developed for CS 360 is a mobile inventory management app designed for warehouse and inventory employees. The main goal of the app is to allow users to create an account, log in, view inventory, add and remove items, update item quantities, and receive an SMS alert when an item's quantity reaches zero. The app was designed to address the need for a simple and efficient way to manage inventory from an Android mobile device.

## User-Centered UI Design

Several screens were necessary to support the needs of the user. The app includes a login and account creation screen, an inventory screen, an add-item screen, and an SMS notification settings screen. The inventory screen displays item names, quantities, and controls for increasing, decreasing, or deleting inventory records.

I kept the user in mind by making common actions easy to find and limiting the number of steps needed to complete a task. Related controls were grouped together, consistent layouts were used between screens, and buttons were sized and positioned so users could interact with them easily. The design was successful because users can move from logging in to managing inventory without unnecessary navigation or complicated menus.

## Development Approach

I approached the coding process by developing the application in smaller sections and testing each section before moving to the next. I first created the SQLite database structure and login functionality. After that, I added the ability to create and display inventory records, followed by updating and deleting inventory items. Finally, I added SMS permission handling and notifications.

Breaking the project into smaller pieces made debugging easier because I could identify which change caused a problem. I would use this same approach in future projects because it reduces the amount of code that needs to be examined when something does not work correctly.

## Testing

I tested the application frequently using the Android Emulator. I tested creating new user accounts, logging in with valid and invalid credentials, adding inventory items, increasing and decreasing quantities, deleting records, and closing and reopening the app to confirm that database information remained stored.

I also tested both outcomes of the SMS permission request. When permission was granted, reducing an inventory item to zero triggered an SMS alert. When permission was denied, the rest of the application continued functioning normally.

Testing was important because it helped identify both functional and interface problems before the application was finalized. It also confirmed that the SQLite database was persistent and that each part of the app worked correctly with the other components.

## Challenges and Innovation

One challenge during development was displaying inventory records dynamically after replacing the sample inventory row that had originally been created during the UI design phase. I needed the screen to display records directly from the SQLite database while also providing separate increase, decrease, and delete buttons for every item.

I solved this by creating the inventory rows dynamically and refreshing the displayed information whenever a user changed the database. I also adjusted the layout proportions and button sizing so that the controls fit properly on a mobile screen without making the inventory grid difficult to read.

## Areas of Success

I was particularly successful with the database and inventory management portion of the application. The app demonstrates all four major CRUD operations: users can create inventory records, read and display stored inventory, update quantities, and delete items.

I also gained experience connecting multiple parts of an Android application together, including activities, XML layouts, SQLite storage, runtime permissions, and SMS functionality. Completing this project gave me a better understanding of the full mobile application development process, from planning and UI design through coding, testing, and final preparation for launch.

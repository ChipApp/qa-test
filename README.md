# QA Test

This is the test for our QA Engineer roles at Chip.

## Test

Using the attached specification [Spec](#spec) you should develop a plan for testing the resulting application. Including plans and tools to collect end user bug report feedback and tools and steps to be taken to provide automated testing and regressions testing on the application resulting from he spec. 

You should time box your test to no more than 2 hours, with the understand this may not allow you enough time to cover everything in through detail, you should priotise those steps you feel most important and triarge the most relevant information. 

## Submit

To submit your test please email all relevant documents to alan@getchip.uk with subject line "QA Engineer - Test"

# Spec

## TODO Mobile Application

This is a simple functional outline for our Android & iOS TODO application, that allows a user to manage a TODO list of items. This is a functional specification for our Mobile apps only and does not indicate how backend implementations of these resources should be constructed.

### Start Screen
- The first screen of our application will show our logo, and two clickable options. "Signup" or "Login"
- Already logged in users will not see this screen
- Clicking on Signup will take users to the signup screen
- Clicking on the Login screen will take users to the Login Screen

### Signup

The user will be presented with three signup options,

- Using email address, password and full name. Email addresses must be validated.
- Using Facebook, no external validation required. Name and email to be taken from Facebook profile.
- Using Twitter, no external validation required. Name and email to be taken from Twitter profile.
- All three options will appear on screen at the same time. 
- If Facebook signup is attempted with an account already registered, the user will be logged into their account.
- If Twitter signup is attempted with an account already registered, the user will be logged into their account.
- If email signup is attempted with an email that ready already exists the user will be redirected to the login screen with a message that this account already exists and a prompt to enter their password, the email field should be filled.

There should also be a link go to login screen.

### Login

The user will be shown the following,

- A field to enter email address
- A field to enter password
- A button to "Login with Email"
- A button to  "Login with Facebook"
- A button to "Login with Twitter"
- If an email login is attempted for a user and the account does not exist, they will be redirected to the signup page with a message that this account does not exist and a prompt they should fill in their details below to complete registration, email address should be filled.
- If a login is attempted from a Facebook account not registered, they should be registered and logged in
- If a login is attempted from a Twitter account not registered, they should be registered and logged in

There should be a link to go to signup.

### Home Screen

Once logged in a user should be shown a home screen, this screen should have the following.

- A list off all items, an item contains "Title, Description, Due Date" all details should be visible.
- If there are no list items a message should display "You have no items todo, click here to add one" with a button that takes you to "Add Item"
- Done items should not appear in the list
- Swiping an item right will mark the item as done
- Pressing and holding on an item will show a menu with "Mark as Done" and "Delete this item" options
- Deleted items should be removed from the list
- The list should be an infinite scroll
- There should be button hovering over he bottom right corner of the list with a plus symbol, clicking this button should take you to the "Add Item" screen

### Add Item

The add item screen should show a form containing the following.

- A field to enter a title
- A textarea to enter a description, this is optional
- A field to enter a due date, this is optional but should be a date in the future
- A button to "Add Item"
- A button to “Cancel”.
- When the Add Item button is pressed the item should be added to the top of the list
- When the cancel item button is pressed the form the clear
- When either button is pressed the form should disappear and reveal the Home screen

### Logout

There should be a button in the top right of the screen at all times called "Logout" when pressed the user should be logged out and returned to our start screen.

## Notes
- This app should be available on all current iPhones and iPads, as well last the last 3 generations.
- This app should be available on all Android devices that support the last 3 major releases of Android.
- This app should work on tablets and mobile phone devices at varying form factors.
- This app should work without in offline mode

Overview
This document outlines the user interface specifications for the User Management Screen, providing details on UI components, behaviors, and initial content displayed to users.

Page Layout

1. Header Section
   Buttons:
   New User: Opens a form for adding a new user.
   Hide Disabled User: A toggle button that hides or shows users who are disabled.
2. User List Table
   Columns:
   ID: Displays the unique identifier for each user.
   User Name: Displays the username of the user.
   Email: Displays the user's email address.
   Enabled: Displays whether the user account is enabled (true) or disabled (false).
   Behavior:
   Clicking on a column header sorts the table by that column.
   The table should support pagination if the user list is extensive.
3. New User Section
   Fields:
   Username: Text input for the user's username.
   Display Name: Text input for the user's display name.
   Phone: Text input for the user's phone number.
   Email: Text input for the user's email address.
   User Roles: Dropdown menu for selecting user roles (e.g., Guest, Admin, SuperAdmin).
   Enabled: Checkbox to enable or disable the user account.
   Behavior:
   When the form is filled out and the "Save User" button is clicked, the new user is added to the list and the form fields are reset.
   If required fields are left blank, display an error message.
   On successful submission, show a confirmation message.
4. Save Button
   Behavior:
   Saves the details of the new or edited user.
   Displays a confirmation message upon successful save.
   Initial View
   When the page is loaded:

The User List Table displays a list of current users.
The "New User" form is empty and ready for input.
Error Handling
If there is a server error or network issue, display a user-friendly error message at the top of the page.
Fields marked as required must not be empty. If they are, display a red asterisk next to the field and an error message below it.
Accessibility
All buttons and form fields should be accessible via keyboard navigation.
Ensure all text has sufficient contrast against the background for readability.

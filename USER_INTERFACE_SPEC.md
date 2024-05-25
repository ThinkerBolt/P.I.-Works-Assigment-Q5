### User Interface Specification Document: User Management Screen


**Components and Layout:**

1. **Top Bar:**
   - **New User Button:** A button labeled "+ New User" that allows the admin to add a new user.
   - **Hide Disabled User Checkbox:** A checkbox labeled "Hide Disabled User" to toggle the visibility of disabled users in the user list.
   - **Save User Button:** A button labeled "Save User" to save the details of the new or edited user.

2. **User List Table:**
   - **Columns:**
     - **ID:** Displays the unique identifier for each user.
     - **User Name:** Displays the username of the user.
     - **Email:** Displays the email address of the user.
     - **Enabled:** Displays the status (true/false) of whether the user is enabled.
   - **Behavior:**
     - Clicking on a column header will sort the table by that column.
     - The table will initially display all users.
     - If the "Hide Disabled User" checkbox is checked, only enabled users will be displayed.

3. **New User Form:**
   - **Fields:**
     - **Username:** Text input for the user's username.
     - **Display Name:** Text input for the user's display name.
     - **Phone:** Text input for the user's phone number.
     - **Email:** Text input for the user's email address.
     - **User Roles:** Dropdown for selecting user roles (options: Guest, Admin, SuperAdmin).
     - **Enabled:** Checkbox to enable or disable the user.
   - **Behavior:**
     - When the "New User" button is clicked, the form will be cleared and ready for input.
     - When the "Save User" button is clicked, the user details will be saved, and the table will be updated.
     - If a user is selected from the table, their details will populate the form for editing.
     - Form validation will ensure all required fields are filled before saving.

**Initial State:**
- The user list table is populated with all users.
- The "Hide Disabled User" checkbox is unchecked.
- The new user form is empty and disabled until "New User" is clicked.

**Additional Behavior:**
- If the "Hide Disabled User" checkbox is checked, the table will refresh to show only enabled users.
- The "Save User" button will be disabled until all required fields in the new user form are filled out correctly.
- Error messages will be displayed if form validation fails upon clicking "Save User".

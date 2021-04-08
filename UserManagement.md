# User Management Screen UI Specification


## _Required functions:_

- View existing users from the table on the left side with their details such as;
    ID, User Name, E-Mail and Enabled
- Add new users to the database by using "New User" button on the header.
- Save user info with "Save User" button on the header.
- Hide disabled users with a toggle selection on the header.
- Enter user information for new users using the form on the right side.

## _How to use the page:_
- User will be greeted with a page that includes;
  1) Header that includes **New User** and **Hide Disabled User** buttons.
    2) A database table that shows ID, UserName, E-Mail and Enabled properties of users, such as;

| ID | UserName | E-Mail | Enabled |
| ------ | ------ | ------ | ------ |
| 1 | AdminUser | admin@piworks.com | true |
| 2 | TestUser | testuser@piworks.com | true |
- **Hide disabled users** button on the header will hide all (Enabled = false) users from the database. It will be able to toggle as the user runs the program.
- By pressing **New User** button, a text form will appear at the right side of the screen. This text form will be filled by the user providing necessary details about new users. These details are;
    **UserName, Display Name, phone, e-mail, user roles and enabled**. When user presses **Save User** button, this form will dissappear until **New User** is pressed again.

## _Restrictions:_
- Functions that manipulalte the database such as **New User** and **Save User** must be only accesible to users with **admin privileges**.
- Database table should be sortable by any property if needed.
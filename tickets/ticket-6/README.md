Ticket: User Management
=======================

**Problem:**

**User Story**

"As a user, I should be able to register for an account, log in, logout, and delete my account."

---

**Task**

For this Ticket, you'll be required to implement all the methods in _usersDao.js_ that are called by the API endpoints in _users.controller.js_. Specifically, you'll implement:

- **getUser**
- **addUser**
- **loginUser**
- **logoutUser**
- **getUserSession**

Registering a new user will insert a document into the **users** collection, and logging in a user will insert a document into the **sessions** collection.

There is a unique index on the **user_id** field in **sessions**, so we can efficiently query on this field.

---

**MFlix Functionality**

Once this ticket is completed, users will be able to register for a new account, log in, logout, and delete their account.

---

**Testing and Running the Application**

Look within the _user-management.test.js_ file to view the unit tests for this ticket.

You can run the unit tests for this ticket by running:

```
npm test -t user-management
```

Once the unit tests are passing, run the application with:

```
npm start
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for User Management?</summary>
   Answer: 5a8d8ee2f9588ca2701894be
</details>
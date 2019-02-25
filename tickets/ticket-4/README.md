Ticket: Paging
==============

**Problem:**

**User Story**

"As a user, I'd like to get the next page of results for my query by scrolling down in the main window of the application."

---

**Task**

Modify the method **getMovies** in _moviesDAO.js_ to allow the application to display new pages of movies.

---

**MFlix Functionality**

The UI is already asking for infinite scroll! You may have noticed a message stating "paging not implemented" when scrolling to the bottom of the page.

Once this ticket is completed, this message will go away, and scrolling to the bottom of the page will result in a new page of movies.

---

**Testing and Running the Application**

Make sure you look at the tests in _paging.test.js_ to look at what is expected.

You can run the unit tests for this ticket by running:

```
npm test -t paging
```

Once the unit tests are passing, run the application with:

```
npm start
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for Paging?</summary>
   Answer: 5a9824d057adff467fb1f526
</details>
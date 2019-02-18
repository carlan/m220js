Ticket: Projection
===========================

**Problem:**

**User Story**

"As a user, I'd like to be able to search movies by country and see a list of movie titles. I should be able to specify a comma-separated list of countries to search multiple countries."

---

**Task**

Implement the **getMoviesByCountry** method in **src/dao/moviesDAO.js** to search movies by country and use projection to return the **title** field. The _id field will be returned by default.

---

**MFlix Functionality**

Once you complete this ticket, the UI will allow movie searches by one or more countries.

---

**Testing and Running the Application**

Make sure to look at the tests in **projection.test.js** to understand what is expected.

You can run the unit tests for this ticket by running:

```
npm test -t projection
```

Once the unit tests are passing, run the application with:

```
npm start
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant unit tests, what is the validation code for Projection?</summary>
   Answer: 5a94762f949291c47fa6474d
</details>
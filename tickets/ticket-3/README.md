Ticket: Subfield Text Search
============================

**Problem:**

**User Story**

"As a user, I'd like to be able to search movies by cast members, genre, or perform a text search of the plot summary, full plot, and title."

---

**Task**

For this ticket, you will need to modify the method **genreSearchQuery** in _moviesDAO.js_ to allow the following movie search criteria:

- genres: finds all movies that match the search genres

The methods for text and cast searches are already implemented:

- _textSearchQuery_: performs a text search in the movies collection
- _castSearchQuery_: finds movies that include any of the wanted cast

You just need to construct the query in **genreSearchQuery** that queries the _movies_ collection by genre. This method should project all document fields.

A text index was created for you when you restored the collections with **mongorestore**, so these queries will be efficient once they are implemented.

**Hint**

Check the implementation of similar formats of search criteria - the _genres_ query should be similar.

---

**MFlix Functionality**

Once you complete this ticket, the UI will allow movie searches by criteria of the **cast**, movie **genres**, movie **title**, and **plot** summary.

---

**Testing and Running the Application**

Make sure to look at the tests in _text_subfield.test.js_ to understand what is expected.

You can run the unit tests for this ticket with:

```
npm test -t text-subfield
```

Once the unit tests are passing, run the application with:

```
npm start
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for Text and Subfield Search?</summary>
   Answer: 5a96a6a29c453a40d04922cc
</details>
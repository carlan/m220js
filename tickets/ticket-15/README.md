Ticket: Handling Timeouts
=========================

**Problem:**

**Task**

For this ticket, you'll be required to modify the connection information for **MongoClient** to set a write concern timeout of **2500** milliseconds.

The **MongoClient** is initialized in the _src/index.js_ file. A link to the [URI connection settings](http://mongodb.github.io/node-mongodb-native/2.1/reference/connecting/connection-settings/) documentation is included here for your reference.
---

**Testing and Running the Application**

_Note:_

> The unit test only has access to DAO methods, but the connection pool size for the MFlix application is set in the _index.js_ file.
>
> However, the connection pool size for the **testing** environment is set in _test/config/mongoEnvironment.js_, so you can test your changes there and the unit test will tell you if something is wrong.
>
> When the unit test passes, make sure to update the code in _src/index.js_ so you can retrieve the validation code from the integration test.

You can run the unit tests for this ticket by running:

```
npm test -t timeouts
```

Once the unit tests are passing, run the application with:

```
npm start
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for Timeouts?</summary>
   Answer: 5addf035498efdeb55e90b01
</details>
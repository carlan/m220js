Final: Question 3
=================

**Problem:**

Suppose an instance of **MongoClient** is created with the _default settings_:

```
import { MongoClient } from "mongodb"

const URI = "mongodb+srv://m220-user:m220-pass@m220-test.mongodb.net/test"

const testClient = await MongoClient.connect(
  URI,
  { connectTimeoutMS: 100, retryWrites: true, useNewUrlParser: true },
)

const clientOptions = testClient.s.options
```

<details> 
  <summary>Which of the following tests will pass?</summary>
   Answer: (X) expect(clientOptions.authSource).toBe("admin")
           (X) expect(clientOptions.retryWrites).toBe(true)
</details>
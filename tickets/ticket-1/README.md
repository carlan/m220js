Ticket: Database Connection
===========================

**Problem:**

**Problem Description**

The MFlix application can't connect to Atlas, so it can't store any data.

---

**Task**

MFlix will use MongoDB as a storage layer, so for this ticket you will build a connection from MFlix to Atlas.

Note: These instructions were included in the **README.rst**. If you already completed the **.env** file, you can skip to **Testing and Running the Application**.

1. First, make sure you've created a user on your Atlas cluster with read and write access to the **mflix** database.

   - The user name should be **m220student** and the password should be **m220password**
   - Don't forget to whitelist your IP address!

2. Copy the connection string. Select that you'd like to connect with Mongo shell, version 3.6 or later. This will give you the **srv** connection string.

3. Locate the file called **dotenv_win** or **dotenv_unix** (depending on your operating system) and replace the information within with your own **srv** connection string:

```
SECRET_KEY=super_secret_key_you_should_change
MFLIX_DB_URI=your_atlas_3.6_srv_connection_uri
MFLIX_NS=mflix
PORT=5000
```

Make sure **not** to wrap your Atlas SRV connection between quotes:

```
MFLIX_DB_URI=mongodb+srv://...
```

* It's highly recommended you also change the **SECRET_KEY** to some very long, very random string. While this application is only meant for local use during this course, software has a strange habit of living a long time.

4. Rename **dotenv_win** or **dotenv_unix** to **.env**. You can do this by running the following command from the mflix-js directory:

```
mv dotenv_unix .env  # on Unix
ren dotenv_win .env  # on Windows
```

Note: Once you rename this file to **.env**, it will no longer be visible in Finder or File Explorer. However, it will be visible from Command Prompt or Terminal, so if you need to edit it again, you can open it from there:

```
vi .env       # on Unix
notepad .env  # on Windows
```

---

**Testing and Running the Application**

In order to reinforce good development practices, everything asked of you in this course is backed up by unit tests. Reading through the tests for a specific exercise will tell you exactly what is expected.

You can run the unit tests for this ticket by running:

```
npm test -t db-connection
```

Once the unit tests are passing, run the application with:

```
npm start
```

Now proceed to the status page to run the full suite of integration tests and get your validation code.

<details> 
  <summary>After passing the relevant tests, what is the validation code for Connection?</summary>
   Answer: 5a9026003a466d5ac6497a9d
</details>


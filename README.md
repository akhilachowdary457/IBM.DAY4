IBM.DAY4
Here is a **clean, professional, and student-friendly README.md content** based on your **Library Management System (Node.js + Express + MongoDB)** project.
You can **directly copy-paste this into your GitHub README.md** 👇



 Library Management System (Backend API)

A simple **Library Management System REST API** built using **Node.js, Express, and MongoDB (Mongoose)**.
This project allows managing books with CRUD operations such as adding books, viewing books, updating copies, changing categories, and deleting books based on conditions.



 Features

* Add multiple books to the database
* View all books
* Filter books by category
* Get books published after a specific year
* Update available copies of a book
* Change book category
* Delete books only when available copies are zero



Technologies Used

* **Node.js**
* **Express.js**
* **MongoDB**
* **Mongoose**
* **REST API**


 Project Structure

```
.
├── app.js               # Main server file
├── bookmodel.js         # Book schema & model
├── db.js                # MongoDB connection
├── package.json         # Project dependencies
├── package-lock.json    # Dependency lock file
```


 Installation & Setup

 Clone the repository

```bash
git clone https://github.com/your-username/library-management-system.git
```

 Install dependencies

```bash
npm install
```

 Start MongoDB

Make sure MongoDB is running locally:

```bash
mongodb://127.0.0.1:27017/libraryDB
```

 Run the server

```bash
node app.js
```

Server will start at:

```
http://localhost:3000
```


 API Endpoints

 Add Books

`POST /addBooks`
Adds a minimum of 7 predefined books.



 Get All Books

`GET /books`



 Get Books by Category

`GET /books/category/:category`

Example:

```
/books/category/AI
```



 Get Books Published After 2015

`GET /books/year/after2015`



 Update Available Copies

`PUT /books/updateCopies/:id`

Request Body:

```json
{
  "change": 2
}
```



  Change Book Category

`PUT /books/changeCategory/:id`

Request Body:

json
{
  "category": "Programming"
}




  Delete Book

`DELETE /books/delete/:id`

> ❗ Book can be deleted **only if availableCopies = 0**



  Testing

You can test all APIs using:

* **Postman**
* **Thunder Client (VS Code)**


 Learning Outcomes

* Hands-on experience with REST APIs
* CRUD operations using MongoDB
* Express routing & middleware
* Mongoose schema and validation



 Author

Dudala Akhila
Student | Developer


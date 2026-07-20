# JSONPlaceholder API Web Application

A web application that integrates the **JSONPlaceholder REST API** to retrieve and create data using HTTP requests. This project demonstrates how a frontend application communicates with a public API, handles responses, and presents data in a user-friendly interface.

## 📌 Project Overview

This project uses **JSONPlaceholder**, a free fake REST API for testing and prototyping applications.

The application can:

* Retrieve posts from the API using GET requests
* Create new posts using POST requests
* Display API data in a clean user interface
* Handle API errors and failed requests

## 🔗 API Used

**JSONPlaceholder**

API Base URL:

```
https://jsonplaceholder.typicode.com
```

Documentation:

```
https://jsonplaceholder.typicode.com/guide/
```

## 🚀 Features

### 1. View Posts

* Fetches existing posts from JSONPlaceholder
* Displays post titles and content
* Uses GET request

Example:

```
GET /posts
```

---

### 2. Create New Posts

* Users can submit a new post
* Sends data to JSONPlaceholder API
* Uses POST request

Example:

```
POST /posts
```

---

### 3. Error Handling

The application handles:

* Failed API requests
* Network errors
* Invalid user input

Users will receive an appropriate error message when something goes wrong.

---

# 🛠 Technologies Used

## Frontend

* HTML
* CSS
* JavaScript

## API

* JSONPlaceholder REST API

## Tools

* Git
* GitHub
* Visual Studio Code

---

# 📂 Project Structure

```
jsonplaceholder-project/

│
├── index.html
├── style.css
├── script.js
│
└── README.md
```

---

# ⚙️ Installation and Setup

## 1. Clone the repository

```bash
git clone (https://github.com/erlsyncc/JSONPlaceholder_API.git
```

---

## 2. Open the project folder

```bash
cd jsonplaceholder_api
```

---

## 3. Run the project

Open:

```
index.html
```

in your browser.

No API key is required because JSONPlaceholder is a free public API.

---

# 🔌 API Integration

## GET Request

The application retrieves posts using:

```
GET https://jsonplaceholder.typicode.com/posts
```

Example response:

```json
{
  "userId": 1,
  "id": 1,
  "title": "sample title",
  "body": "sample content"
}
```

---

## POST Request

The application creates a new post using:

```
POST https://jsonplaceholder.typicode.com/posts
```

Example request:

```json
{
  "title": "New Post",
  "body": "This is a new post",
  "userId": 1
}
```

---

# 📖 Available Resources

JSONPlaceholder provides several fake resources:

| Resource | Endpoint    |
| -------- | ----------- |
| Posts    | `/posts`    |
| Comments | `/comments` |
| Albums   | `/albums`   |
| Photos   | `/photos`   |
| Todos    | `/todos`    |
| Users    | `/users`    |

---

# 🧪 Testing API

Example GET request:

```javascript
fetch("https://jsonplaceholder.typicode.com/posts")
.then(response => response.json())
.then(data => console.log(data));
```

Example POST request:

```javascript
fetch("https://jsonplaceholder.typicode.com/posts", {
    method: "POST",
    body: JSON.stringify({
        title: "Hello API",
        body: "Testing POST request",
        userId: 1
    }),
    headers:{
        "Content-type":"application/json"
    }
})
.then(response => response.json())
.then(data => console.log(data));
```

---

# 📌 Notes

* JSONPlaceholder is a testing API.
* POST, PUT, PATCH, and DELETE requests simulate database operations but do not permanently save changes.
* No authentication token or API key is required.

---

# 👨‍💻 Developers

Created by:

- Combenido, Earlsin Mae G.
- Consigo, Rica Mae G.
- Tariao, Bernadette B.

---

# 📄 License

This project is created for educational purposes.

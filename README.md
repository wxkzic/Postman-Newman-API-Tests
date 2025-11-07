# 🧪 postman-api-tests

This project contains automated API tests built with **Postman** and executed through **Newman** with HTML reporting enabled.  
It demonstrates practical skills in **REST API testing**, working with **variables**, **request chaining**, and automated test execution in local or CI/CD environments.

---

## 🚀 Technologies Used

| Technology | Purpose |
|-----------|---------|
| **Postman** | Creating and debugging API requests |
| **Newman** | Command-line runner for executing Postman collections |
| **newman-reporter-htmlextra** | Generates extended HTML reports |
| **Node.js** | Runtime environment for executing Newman and dependencies |

---

## 🧱 Test Coverage Overview

The test suite performs CRUD operations on the JSONPlaceholder API:

| Test Name | Method | Endpoint | Verified Behavior |
|----------|--------|----------|------------------|
| **Create Post** | `POST` | `/posts` | Status `201`, response contains `id`, store `postId` for later use |
| **Update Post** | `PUT` | `/posts/{postId}` | Status `200`, response `id` matches stored `postId` |
| **Delete Post** | `DELETE` | `/posts/{postId}` | Status `200`, response body equals `{}` |

---

## ⚙️ Setup

```bash
git clone <repository-url>
cd postman-api-tests
npm install
```
---

## ▶️ Run Tests

```bash
npm run test

reports/newman.html

start reports/newman.html     # Windows

open reports/newman.html      # macOS

xdg-open reports/newman.html  # Linux
```
---

## 📊 Example of Report Output

The htmlextra reporter generates a user-friendly dashboard containing:

Total requests

Passed / failed assertions

Execution times and payload sizes

Detailed request/response breakdown

This format is suitable for QA documentation, bug reporting, and CI/CD logs.

---

## ✅ Purpose of This Project

This project is designed to:

Demonstrate API automation testing skills

Show ability to chain requests and validate dynamic data

Produce clean and visual test execution reports

Serve as part of a professional QA portfolio

---

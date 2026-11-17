# 🧪 QA API Testing Portfolio — ReqRes

This repository contains a REST API test suite developed in **Postman** to validate CRUD operations, authentication flows, dynamic environment variables, and negative test scenarios.

## 🎯 Test Scenarios Covered
* **GET `/api/users?page=2`** — Validates paginated data retrieval, `200 OK` status code, and JSON response integrity.
* **POST `/api/users`** — Validates record creation with JSON payload, `201 Created` status code, and dynamic extraction of the generated `id` into an environment variable.
* **PUT `/api/users/2`** — Validates user profile updates and verifies updated fields in the `200 OK` response.
* **DELETE `/api/users/2`** — Validates record deletion and empty response body (`204 No Content`).
* **POST `/api/login` (Negative Test)** — Attempts authentication without a password to confirm proper API error handling (`400 Bad Request` with `"Missing password"` error message).

## 🛠️ How to Run
1. Import `ReqRes - QA Portfolio.postman_collection.json` and `ReqRes Env.postman_environment.json` into **Postman**.
2. Select **`ReqRes Env`** in the top-right environment dropdown.
3. Add a free API key from [reqres.in](https://reqres.in) under the collection's **Authorization** tab (`x-api-key`).
4. Run requests individually or via the **Collection Runner** to inspect the automated test assertions.

# Github-API-Testing-Postman-
# 🚀 API Testing Automation Project (Postman & Newman)

This repository contains end-to-end API test automation scripts built using **Postman** and executed via **Newman CLI** to generate detailed HTML test execution reports. The test suite covers both **Positive** and **Negative** testing scenarios across multiple HTTP methods.

---

## 📌 Project Overview
- **Target API:** `[Enter API Name, e.g., ReqRes API / GitHub REST API / E-Commerce API]`
- **Base URL:** `[Enter Base URL, e.g., https://api.example.com]`
- **Testing Type:** Functional API Testing, Positive & Negative Testing, Status Code & Response Validation
- **Reporting:** Automated HTML Report generated using Newman

---

## 🧪 HTTP Methods & Test Scenarios Covered

### 1. HTTP Methods Tested
- **GET:** Fetching single and multiple resource details.
- **POST:** Creating new records with valid and invalid payloads.
- **PUT / PATCH:** Updating existing resource data.
- **DELETE:** Removing existing resources and verifying deletion.

### 2. Positive Test Cases ✅
- Validating successful status codes (`200 OK`, `201 Created`, `204 No Content`).
- Verifying response body structure, JSON keys, and accurate data values.
- Validating response headers (`Content-Type`, `Authorization`) and response time (`< 1000ms`).
- Dynamic variable chaining (extracting `ID` or `Token` from one response and passing it to the next request).

### 3. Negative Test Cases ❌
- Sending requests with missing or invalid authentication tokens (`401 Unauthorized`).
- Passing invalid or missing mandatory fields in the request body (`400 Bad Request`).
- Requesting non-existent resource IDs or wrong endpoints (`404 Not Found`).
- Sending unsupported HTTP methods or malformed JSON payloads (`405 Method Not Allowed` / `422 Unprocessable Entity`).

---

## 📂 Repository Structure

```text
├── Collection/
│   └── API_Testing_Collection.json      # Exported Postman Collection with test assertions
├── Environment/
│   └── API_Environment.json             # Environment variables (Base URL, Tokens, IDs)
├── Reports/
│   └── Newman_Test_Report.html          # Generated HTML execution report
└── README.md                            # Project documentation

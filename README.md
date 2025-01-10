# KoinX Backend Internship Assignment

This repository contains the implementation of the backend tasks required for the **KoinX Backend Internship Assignment**. The project includes a server-side application built with **Node.js** and **MongoDB** to fulfill the outlined tasks.

---

## 🚀 Deployment  
The application is deployed and accessible at: [https://koinx-assignment-arnav-sao.vercel.app/](https://koinx-assignment-arnav-sao.vercel.app/)

---

## 📌 Objective  
To develop a backend application capable of:  
1. Fetching cryptocurrency data periodically and storing it in the database.  
2. Providing APIs for cryptocurrency statistics and price deviation analysis.

---

## 🛠️ Tasks  

### Task 1: Background Job  
- **Description:**  
  A background job runs every 2 hours to fetch the following details for three cryptocurrencies (`bitcoin`, `matic-network`, `ethereum`):  
  - Current price in USD  
  - Market cap in USD  
  - 24-hour change (%)  

- **Data Source:**  
  Fetched from the [CoinGecko API](https://docs.coingecko.com/v3.0.1/reference/introduction).

- **Database:**  
  The fetched data is stored in MongoDB.  

---

### Task 2: API - `/stats`  
- **Endpoint:** `/stats`  
- **Query Parameters:**  
  ```json
  {
      "coin": "bitcoin" // Could be one of: bitcoin, matic-network, ethereum
  }

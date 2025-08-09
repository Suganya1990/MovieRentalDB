# 🎦 Movie Rental MongoDB Project

This project contains scripts to create and populate a movie rental database using MongoDB. It includes collection setup, data insertion, and sample queries.

---

## 📁 Project Structure

```bash
movie-rental/
├── dbCollectionScript.txt      # MongoDB collection creation scripts
├── customerScript.txt          # Insert customer data
├── movieScript.txt             # Insert movie data
├── employeeScript.txt          # Insert employee data
├── rentalScript.txt            # Insert rental data
├── orderScript.txt             # Insert order data
├── paymentScript.txt           # Insert payment data
├── queryExamples.txt           # Sample queries
└── README.md                   # Project setup guide (this file)
```

---

## 🚀 Setup Instructions

### 1. 🛠 Install MongoDB
Ensure you have MongoDB and `mongosh` installed. You can download from:  
https://www.mongodb.com/try/download/community

---

### 2. 🔧 Create the Database

1. Open **PowerShell** or **Command Prompt**
2. Start MongoDB shell:
   ```bash
   mongosh
   ```
3. Switch to your database (this will create it):
   ```js
   use movie_rental
   ```
4. (Optional) Verify:
   ```js
   show dbs
   ```

---


## 🧾 Data Insertion Scripts

Repeat the following steps for each data file:

### ➕ Insert Customers
```bash
mongosh
use movie_rental
```
Paste contents from `customers.txt`

---

### ➕ Insert Movies
```bash
mongosh
use movie_rental
```
Paste contents from `movies.txt`

---

### ➕ Insert Employees
```bash
mongosh
use movie_rental
```
Paste contents from `employees.txt`

---

### ➕ Insert Rentals
```bash
mongosh
use movie_rental
```
Paste contents from `rentals.txt`

---


## 🔍 Sample Querying

You can find examples of update, find, and aggregate queries in `queries.txt`.  
Example:
```js
// Find all customers over age 30
db.customers.find({ date_of_birth: { $lt: new Date("1994-01-01") } })
```

---

## ✅ Notes

- The database is built for a single-branch movie rental company
- Each collection has validation structure as per schema
- Make sure the MongoDB service is running before launching `mongosh`

---

## 📧 Contact

For questions or issues, please contact: [suganyamaheswaran@gmail.com]

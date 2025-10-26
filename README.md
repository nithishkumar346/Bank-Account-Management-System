# 🏦 Bank Account Management System  

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![SQLite](https://img.shields.io/badge/Database-SQLite-green?logo=sqlite)
![Status](https://img.shields.io/badge/Status-Active-success)
![License](https://img.shields.io/badge/License-MIT-orange)

---

## 📘 Overview  
The **Bank Account Management System** is a Python-based console application designed to simulate core banking operations.  
It enables you to manage **customers**, **accounts**, and **transactions** efficiently, all stored securely in an **SQLite database**.  

This project demonstrates practical implementation of **CRUD operations**, **database management**, and **transactional logic** in Python — perfect for beginners and learners.

---

## 🚀 Features  

✅ **Customer Management** – Add, view, update, and delete customer records.  
✅ **Account Management** – Open and close accounts linked to customers.  
✅ **Transactions** – Deposit, withdraw, and transfer funds between accounts.  
✅ **Reports** – Generate transaction history and monthly statements.  
✅ **Search** – Find accounts by customer name.  
✅ **Data Persistence** – All data stored using SQLite for reliability.  

---

## 🧠 Tech Stack  

| Component | Technology |
|------------|-------------|
| **Language** | Python 3.x |
| **Database** | SQLite |
| **Libraries Used** | `sqlite3`, `datetime` |

---

## 🧩 Database Schema  

### 🧑‍💼 Customers Table  
| Field | Type | Description |
|--------|------|-------------|
| `customer_id` | INTEGER (PK) | Unique ID for each customer |
| `name` | TEXT | Customer name |
| `email` | TEXT | Customer email |
| `phone` | TEXT | Customer phone number |

### 💳 Accounts Table  
| Field | Type | Description |
|--------|------|-------------|
| `account_id` | INTEGER (PK) | Unique ID for each account |
| `customer_id` | INTEGER (FK) | Linked customer ID |
| `account_type` | TEXT | Account type (Savings/Current) |
| `balance` | REAL | Account balance |
| `created_date` | TEXT | Account creation date |

### 💰 Transactions Table  
| Field | Type | Description |
|--------|------|-------------|
| `transaction_id` | INTEGER (PK) | Unique transaction ID |
| `account_id` | INTEGER (FK) | Associated account |
| `type` | TEXT | Transaction type (Deposit/Withdraw/Transfer) |
| `amount` | REAL | Transaction amount |
| `date` | TEXT | Transaction timestamp |
| `description` | TEXT | Details of the transaction |

---

## ⚙️ Installation & Setup  

1️⃣ **Clone this repository**
```bash
git clone https://github.com/your-username/bank-management-system.git
cd bank-management-system

# 🎬 Maven Movies Rental Business — SQL Data Analysis Project

An end-to-end SQL portfolio project analyzing operational data for a DVD/movie rental business using the **Maven Movies** dataset. This project demonstrates practical SQL skills through exploratory data profiling, schema discovery, and a series of realistic ad-hoc business questions that a rental company's marketing, inventory, and management teams might ask.

---

## 📌 Project Overview

This project applies SQL to analyze the **MAVENMOVIES** database — a relational dataset modeling a multi-store movie rental business. The analysis moves from basic exploratory queries into grouped, filtered, and CASE-based business analysis, answering real questions like:

- Which customers should be rewarded for loyalty?
- Which titles and stores drive the most revenue?
- How should the film catalog be organized for recommendations and reporting?
- Which films should be stocked more at a specific store?

---

## 🛠️ Tools Used

- **SQL (MySQL)**
- **MySQL Workbench**

---

## 📂 Dataset Description

The `MAVENMOVIES` schema models a multi-store movie rental business, structured as a set of related tables covering customers, films, inventory, rentals, payments, staff, and cast.

**Key Tables:**

| Table | Description |
|---|---|
| `CUSTOMER` / `ADDRESS` | Customer profiles, contact details, and home store assignment |
| `FILM` / `CATEGORY` / `LANGUAGE` / `FILM_CATEGORY` | Film catalog, genres, and language |
| `ACTOR` / `FILM_ACTOR` | Cast members and which films they appear in |
| `INVENTORY` | Physical copies of each film, tied to a specific store |
| `RENTAL` | Individual rental transactions (who rented what, and when) |
| `PAYMENT` | Payments tied to rentals and customers |
| `STAFF` / `ADVISOR` | Employees and advisors associated with the business |

---

## 📊 Project Structure

The SQL script is organized into 7 major sections, moving from basic exploration to advanced business analysis:

### 1️⃣ Basic Dataset Overview & EDA
Initial exploration of the schema, catalog pricing, and rating composition.
- Customer contact list for marketing
- Movie counts by rental rate
- Rating distribution across the catalog and per store
- Master catalog list (title, category, language)

### 2️⃣ Rental Activity & Revenue Analysis
Identifying which titles, customers, and stores drive the most rental activity and revenue.
- Rental count per film (popularity ranking)
- Top 10 grossing titles
- Top spending customer (loyalty candidate)
- Revenue by store
- Monthly rental trends
- Customers with 30+ rentals (rewards list)

### 3️⃣ Customer Filtering & Engagement
Ad-hoc filtering requests and identifying low-engagement customers.
- Payment history filtering by customer ID, amount, and date
- Films with "Behind the Scenes" special features
- Customers with fewer than 15 lifetime rentals (win-back list)

### 4️⃣ Film Catalog Analysis
Understanding pricing, duration, and using `CASE` logic to segment the catalog.
- Film counts by rating and rental duration
- Correlation between replacement cost and rental rate
- Runtime bucket classification
- Multi-condition CASE logic for family-friendly recommendations

### 5️⃣ Store & Customer Status Reporting
Labeling customer accounts by store/active status and auditing inventory.
- Store + active status labels per customer
- Full inventory listing by store

### 6️⃣ Actor & Cast Analysis
Understanding cast size per film and building an actor-to-filmography lookup.
- Number of films per actor
- Number of actors per film
- Full actor-to-title filmography list

### 7️⃣ Store Expansion & Staff Reporting
Supporting collection-expansion decisions and combining staff/advisor rosters.
- Store 2 inventory audit for expansion planning
- Combined staff + advisor directory using `UNION`

---

## 💡 SQL Concepts Demonstrated

- Multi-table

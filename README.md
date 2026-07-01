🎬 Maven Movies Rental Business — SQL Data Analysis Project

An end-to-end SQL portfolio project analyzing operational data for a DVD/movie rental business using the Maven Movies dataset. This project demonstrates practical SQL skills through exploratory data profiling, schema discovery, and a series of realistic ad-hoc business questions that a rental company's marketing, inventory, and management teams might ask.


📌 Project Overview

This project applies SQL to analyze the MAVENMOVIES database — a relational dataset modeling a multi-store movie rental business. The analysis moves from basic exploratory queries into grouped, filtered, and CASE-based business analysis, answering real questions like:


Which customers should be rewarded for loyalty?
Which titles and stores drive the most revenue?
How should the film catalog be organized for recommendations and reporting?
Which films should be stocked more at a specific store?



🛠️ Tools Used


SQL (MySQL)
MySQL Workbench



📂 Dataset Description

The MAVENMOVIES schema models a multi-store movie rental business, structured as a set of related tables covering customers, films, inventory, rentals, payments, staff, and cast.

Key Tables:

TableDescriptionCUSTOMER / ADDRESSCustomer profiles, contact details, and home store assignmentFILM / CATEGORY / LANGUAGE / FILM_CATEGORYFilm catalog, genres, and languageACTOR / FILM_ACTORCast members and which films they appear inINVENTORYPhysical copies of each film, tied to a specific storeRENTALIndividual rental transactions (who rented what, and when)PAYMENTPayments tied to rentals and customersSTAFF / ADVISOREmployees and advisors associated with the business


📊 Project Structure

The SQL script is organized into 7 major sections, moving from basic exploration to advanced business analysis:

1️⃣ Basic Dataset Overview & EDA

Initial exploration of the schema, catalog pricing, and rating composition.


Customer contact list for marketing
Movie counts by rental rate
Rating distribution across the catalog and per store
Master catalog list (title, category, language)


2️⃣ Rental Activity & Revenue Analysis

Identifying which titles, customers, and stores drive the most rental activity and revenue.


Rental count per film (popularity ranking)
Top 10 grossing titles
Top spending customer (loyalty candidate)
Revenue by store
Monthly rental trends
Customers with 30+ rentals (rewards list)


3️⃣ Customer Filtering & Engagement

Ad-hoc filtering requests and identifying low-engagement customers.


Payment history filtering by customer ID, amount, and date
Films with "Behind the Scenes" special features
Customers with fewer than 15 lifetime rentals (win-back list)


4️⃣ Film Catalog Analysis

Understanding pricing, duration, and using CASE logic to segment the catalog.


Film counts by rating and rental duration
Correlation between replacement cost and rental rate
Runtime bucket classification
Multi-condition CASE logic for family-friendly recommendations


5️⃣ Store & Customer Status Reporting

Labeling customer accounts by store/active status and auditing inventory.


Store + active status labels per customer
Full inventory listing by store


6️⃣ Actor & Cast Analysis

Understanding cast size per film and building an actor-to-filmography lookup.


Number of films per actor
Number of actors per film
Full actor-to-title filmography list


7️⃣ Store Expansion & Staff Reporting

Supporting collection-expansion decisions and combining staff/advisor rosters.


Store 2 inventory audit for expansion planning
Combined staff + advisor directory using UNION



💡 SQL Concepts Demonstrated


Multi-table JOINs (INNER, LEFT)
Aggregate functions (COUNT, SUM, AVG, MIN, MAX)
GROUP BY and HAVING clauses
Subqueries and derived tables
CASE-based segmentation and classification
Pattern matching with LIKE
Set operations (UNION)
Filtering with WHERE, logical operators (AND, OR, IN)



🔑 Key Findings & Business Takeaways

Catalog & Pricing


Rental rate, rating, and rental-duration breakdowns give a full picture of catalog pricing and organization.
CASE-based logic enables auto-tagging of films for merchandising and family-friendly recommendations.


Rentals & Revenue


Rental counts and top-10 grossing titles identify the best-performing inventory.
Revenue attribution by store reveals the stronger-performing location.
Monthly rental trends expose seasonal demand patterns for staffing and promotions.


Customers


Top spenders and 30+ rental "loyal customers" are natural targets for a rewards program.
Customers with fewer than 15 lifetime rentals form a win-back / re-engagement segment.


Cast & Inventory


Actor-to-film queries support a "browse by actor" feature and give investors visibility into production scale.
Store 2 inventory analysis directly supports collection-expansion planning.



📁 Repository Contents

├── maven_movies_analysis.sql   # Full SQL script with all 31 business queries
├── README.md                   # Project documentation (this file)


🚀 How to Run


Set up the MAVENMOVIES database in MySQL Workbench (or your preferred MySQL client).
Run the queries in maven_movies_analysis.sql sequentially, or execute individual sections as needed.
Results will populate directly from your live database instance.



👩‍💻 Author

Payal Rana
B.Tech Graduate | Aspiring Data Analyst


🔗 Related Projects

This project pairs with an accompanying Amazon Sales SQL Project, showcasing SQL-based data analysis across two different business domains.




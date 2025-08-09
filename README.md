# 📺 OTT Database Management System

## 📌 Project Overview

This project is a **OTT Platform Database** designed to store, manage, and query comprehensive data for an Over-The-Top (OTT) streaming service.
It includes:

* Database schema in **BCNF** for optimal normalization and minimal redundancy.
* **ER Diagram** & **Relational Schema Diagram**.
* **DDL scripts** for database creation.
* **Sample data insertion scripts**.
* **SQL queries** for analytics and reporting.

---

## 📂 Project Structure

| File Name                 | Description                                                                                    |
| ------------------------- | ---------------------------------------------------------------------------------------------- |
| `DDL_Scripts.txt`         | Contains SQL statements to create the database schema, tables, constraints, and relationships. |
| `Data_Insert_Scripts.txt` | Sample data population scripts for testing and demonstration.                                  |
| `SQL_Queries.txt`         | Collection of analytical and reporting queries.                                                |
| `BCNF_Proof.pdf`          | Proof that all relations are in **Boyce-Codd Normal Form**.                                    |
| `ER_Daigram.pdf`          | Entity-Relationship diagram of the database.                                                   |
| `Relational_Diagram.pdf`  | Relational schema representation of the database.                                              |

---

## 🗄 Database Schema Overview

The schema models the following main entities:

* **Production Companies** (`Production`)
* **Content Information** (`Content`, `Movies`, `Shows`, `TV_Series`, `Episode`)
* **Users & Watchlists** (`Ott_User`, `Watchlist`)
* **Streaming Records** (`Streams`)
* **Genres, Audio, Subtitles** (`Content_Genre`, `Content_Audio`, `Content_Subtitle`)
* **Actors & Cast** (`Actor`, `Content_Cast`, `Starred_in`)
* **Advertisements** (`Advertisement`, `Advertise_Genre`, `Displayed_IN`)
* **Statistics & Analytics** (`Statistics`, `Related_Shows`)

All relationships are enforced via **foreign key constraints** with `ON DELETE CASCADE` and `ON UPDATE CASCADE`.

---

## 📊 Normalization

All relations are verified to be in **BCNF** as shown in `BCNF_Proof.pdf`.
This ensures:

* No redundancy
* No anomalies (insertion, update, deletion)
* Strong dependency preservation

---

## 📚 Technologies Used

* **PostgreSQL** – Database Engine
* **SQL** – Query Language
* **BCNF** – Database Normalization Standard

---

## 👨‍💻 Author

Developed as part of a **Database Management Systems** project to demonstrate relational schema design, normalization, and analytics for an OTT streaming platform.

---

📘 Project Overview — Loan Collateral Management System


The Loan Collateral Management System is a database-driven project designed to help financial institutions register, track, monitor, and manage collateral provided by customers when securing loans.
The system ensures proper recording of collateral items, valuation details, loan–collateral relationships, and security monitoring.

This project focuses on database development using Oracle 19c, following the requirements and phases provided during the coursework.

🎯 2. Project Objectives

The main objectives of the system are:

✔ Maintain accurate customer records

✔ Register and track collateral items

✔ Store loan details and associate loans with collateral

✔ Ensure secure database storage using tablespaces

✔ Provide role-based access through a dedicated admin user

✔ Offer structured documentation and scripts for consistent deployment

This project aims to demonstrate practical skills in database design, SQL development, and Oracle PDB management.

🗃️ 3. System Modules

The system is built around four major data components:

1. Customers

Stores customer personal information (name, contact, ID type, etc.)

2. Loans

Records loan applications, approval status, and loan amounts.

3. Collateral

Keeps details about collateral items (type, value, status).

4. Loan–Collateral Relationship

Links collateral to loans using foreign keys.

🧱 4. Database Architecture
✔ Pluggable Database (PDB)

A dedicated PDB named:
B_28450_Odry_loanCollateral_DB

This ensures full isolation from other environments.

✔ Custom Tablespaces

To improve performance and structure:

coll_data → Stores data tables

coll_index → Stores indexes

coll_temp → Used for sorting & temporary operations

✔ Dedicated Admin User

The PDB uses a custom administrator:

Username: ODRY_ADMIN

Password: Odry

Roles: CONNECT, RESOURCE, PDB_DBA

Quotas: Unlimited on coll_data & coll_index

This ensures secure and controlled access within the PDB.

📝 5. Project Deliverables

This repository contains:

🔹 Database Creation Scripts

Create pluggable database

Create tablespaces

Create user and grant privileges

🔹 Data Definition Scripts (DDL)

Tables

Primary & foreign keys

Indexes

Sequences & triggers

🔹 Sample Data Scripts (DML)

Insert sample customers, loans, collateral items, etc.

🔹 ER Diagram

A full entity-relationship diagram showing the tables and relationships.

🔹 Readme Documentation

Setup steps, system explanation, and project structure breakdown.

```📂 6. Project Structure
Loan-Collateral-Management-System/
Loan-Collateral-Management-System/
│
├── documentation/
│   ├── README.md
│   ├── project_overview.md
│   └── database_setup.md
│
├── sql/
│   ├── 01_create_pdb.sql
│   ├── 02_tablespaces.sql
│   ├── 03_user_setup.sql
│   ├── 04_create_tables.sql
│   ├── 05_insert_data.sql
│   └── 06_test_queries.sql
│
├── diagrams/
│   ├── ERD.png
│   └── Dataflow.png
│
└── LICENSE
```

🧪 7. Testing

Testing includes:

Table creation validation

Foreign key integrity checks

Insertion of sample records

Queries to retrieve loan and collateral details




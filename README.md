# IT Help Desk Ticket Management Database

## Project Overview
This repository contains a clean, production-ready relational database schema designed for an **IT Help Desk Management System**. The project simulates real-world IT support operations, focusing on tracking user issues, categorizing priorities, managing technician availability (L1/L2/L3 support tiers), and calculating internal operational metrics.

## Technical Core Features
* **Relational Schema Design:** Implemented normalized tables (`USERS`, `TECHNICIANS`, `TICKETS`) utilizing strict data integrity controls, explicit checking constraints, and structured Primary/Foreign key relations.
* **Analytical Business Logic:** Formulated structural multi-table `LEFT JOIN` queries optimized for extraction of critical SLA-breaching data.
* **PL/SQL Programming:** 
  * Designed a modular **Stored Function** (`get_tech_open_tickets`) to programmatically calculate active ticket loads per technician.
  * Developed a **Database Trigger** (`trg_set_resolved_date`) to automate operational timestamp logging during object state transition updates.

## Language & Environment
* **Language:** Oracle SQL & PL/SQL
* **Platform Compatibility:** Oracle Database Enterprise Edition

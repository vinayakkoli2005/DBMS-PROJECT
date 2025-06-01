]
# 🐾 Animal Adoption & Welfare Management System

A comprehensive Database Management System (DBMS) built for the **Animal Welfare Organization (AWO)** to streamline the handling of animal rescues, adoptions, medical care, lost & found cases, fostering, pet licensing, donations, and staff management.

---

## 📌 Table of Contents

* [Project Overview](#project-overview)
* [Features](#features)
* [Tech Stack](#tech-stack)
* [Database Design](#database-design)
* [Modules Description](#modules-description)
* [How to Use](#how-to-use)
* [Screenshots (if applicable)](#screenshots-if-applicable)
* [Team Members](#team-members)
* [Future Enhancements](#future-enhancements)

---

## 📖 Project Overview

The Animal Welfare Organization (AWO) needed a centralized system to efficiently manage the intake, care, adoption, and legal processing of rescued animals. This DBMS project is designed to handle complex workflows, ensure compliance with regulations, and support community involvement through reporting, donations, and pet licensing.

---

## ✅ Features

1. **Animal Rescue & Shelter Management**

   * Register rescued animals with species, age, breed, and medical condition
   * Track shelter capacity and relocate animals as needed
   * Monitor quarantine and recovery progress

2. **Lost & Found Matching**

   * Match rescued animals with reported lost pets
   * Owner verification via photos and medical records

3. **Emergency Rescue Reporting**

   * Allow public users to report cases online
   * Status tracking (Pending, In Progress, Rescued)
   * Notify the nearest rescue team

4. **Adoption Workflow**

   * Search animals by species, breed, health status
   * Submit adoption requests with identity proof
   * Interview scheduling, eligibility checks, adoption certificate generation

5. **Medical & Veterinary Records**

   * Store medical history, vaccinations, surgeries
   * Automatic reminders for vaccinations and appointments

6. **Pet Licensing**

   * Apply for licenses with pet and medical details
   * Generate Pet License Numbers (PLN) and renewal alerts

7. **Donations & Sponsorships**

   * Accept public or organizational donations
   * Generate thank-you emails and financial reports

8. **Staff Management**

   * Register staff and assign shelters
   * Track tasks like feeding, cleaning, walking

---

## 🛠️ Tech Stack

* **Database:** MySQL
* **Languages:** SQL, PHP (for simulation), HTML/CSS
* **Modeling Tools:** ERD Diagram, Relational Schema
* **IDE:** MySQL Workbench, Visual Studio Code

---

## 🗂️ Database Design

* Normalized up to 3NF
* Created **10+ tables** including:

  * `Animals`, `Adopters`, `Shelters`, `RescueReports`, `VeterinaryRecords`, `Licenses`, `Donations`, `Staff`, etc.
* Relationships:

  * One-to-many (Shelter to Animal)
  * Many-to-many (Adopter ↔ Animal via Adoption table)
  * One-to-one (Animal ↔ Medical record)

---

## 🔍 Modules Description

| Module          | Description                                                       |
| --------------- | ----------------------------------------------------------------- |
| `Animal`        | Stores animal details including ID, species, breed, health status |
| `Shelter`       | Tracks capacity, address, and associated animals                  |
| `Adoption`      | Links adopters and animals, with verification status              |
| `Medical`       | Includes vaccination and treatment records                        |
| `RescueReports` | Logs public reports with timestamps and locations                 |
| `Donations`     | Tracks amount, donor details, and receipts                        |
| `Licenses`      | Records legal pet ownership with renewal reminders                |
| `Staff`         | Assigns employees to shelters with roles and task logs            |

---

## 🚀 How to Use

1. **Set up the database:**

   * Import the provided `.sql` file into MySQL Workbench or another MySQL tool.
   * Create all tables and enforce foreign key constraints.

2. **Run simulation (optional):**

   * Use the HTML/CSS/PHP files to simulate user input (e.g., submitting rescue or adoption forms).

3. **Query and Analyze:**

   * Run SQL queries to insert, update, retrieve, and analyze data related to animal welfare operations.

---

## 👥 Team Members

* Vaibhav Sorot
* Ronak Gupta
* Yashasvi
* **Vinayak Koli**

---

## 🔮 Future Enhancements

* Add user authentication and login for staff and admins
* Build a real-time map integration for rescue locations
* Integrate email/SMS notifications for adopters and donors
* Develop full-stack web app with backend in Django or Node.js
* Deploy on cloud (e.g., AWS RDS + frontend on Netlify)



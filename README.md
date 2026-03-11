<div align="center">
  <h1>🏨 C++ Hotel Management System (OOP)</h1>
  <p>A comprehensive console-based application built in C++ to demonstrate Object-Oriented Programming principles through hotel administration.</p>
</div>

---

## 📌 Short Description
Developed for the **Object-Oriented Programming (OOP)** course (Year 1), this project simulates a fully functional Hotel Management System. It provides interactive CLI menus for both Clients and Administrators, allowing dynamic management of bookings, room availability, and hotel staff. The system persistently stores data using file I/O operations, ensuring data is not lost between sessions.

## 💻 Tech Stack & Concepts
![C++](https://img.shields.io/badge/C++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white)

This project heavily emphasizes core OOP principles:
* **Inheritance:** A base `Persoana` class is extended by `Client` and `Angajat`. The `Angajat` class is further specialized into sub-roles like `Bucatar`, `Ingrijitor`, `Receptioner`, and `Manager`.
* **Polymorphism:** Staff members are managed through a unified vector of pointers (`std::vector<Angajat*>`), utilizing `dynamic_cast` at runtime to access role-specific behaviors (e.g., extracting specific attributes like a Chef's certifications when exporting to files).
* **Encapsulation:** All class attributes are protected and strictly accessed via Getter and Setter methods to maintain state integrity.
* **Abstraction:** The central orchestration `Hotel` class aggregates instances of `Camera`, `Rezervare`, `Client`, and `Angajat` to run the entire system.

## ✨ Key Features

* **👥 Interactive User Roles:** Dedicated menu flows for `Client` (view rooms, book, leave reviews) and `Administrator` (manage staff, view all bookings).
* **💼 Advanced HR Management:** Admins can hire or fire staff, dynamically adjust salaries (`MaresteSalariuAdmin`, `MicsoreazaSalariuAdmin`), and view global HR statistics. Each staff role has unique traits (e.g., `Ingrijitor` manages specific floors, `Bucatar` holds an array of specialized certifications).
* **🛏️ Booking Engine:** Handles room assignment, calculates total prices, applies dynamic discounts (`CalcularePretDupaDiscount`), and tracks different payment methods.
* **💾 Data Persistence:** The state of the hotel (rooms, bookings, staff, clients) is automatically loaded from and serialized back to text files during execution.

## 🚀 Setup & Execution

**1. Clone the repository:**
```bash
git clone 
cd 
```

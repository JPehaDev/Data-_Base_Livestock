# **Livestock Data Manager (Java + Excel)**

A desktop system built with **Java** to manage cattle information on farms (identification, sex, weight, breed/color, inventories, and movements), with export to **Excel** for easy reporting and administration. The goal is to provide a lightweight, cost-free alternative to organize herd data, enabling quick searches by animal number and generation of files with key data.

> This repository is a **fork** of the original project _Base-de-Datos-con-Excel-MACC_. It preserves the spirit of creating an accessible tool to support queries, monthly inventories, and registration of purchases, sales, or losses (deaths) with output to Excel.

---

## 🧭 Table of Contents

- [Features](#-features)
- [Requirements](#-requirements)
- [Installation](#-installation)
- [Usage](#-usage)
- [Project Structure](#-project-structure)
- [Roadmap](#-roadmap)
- [Contributing](#-contributing)
- [License](#-license)
- [Credits](#-credits)

---

## ✨ Features

- **Animal management:** register ID, sex, weight, breed/color.  
- **Instant search:** retrieve data by entering an animal number.  
- **Monthly inventories:** support for periodic updates of herd counts and weights.  
- **Herd movements:** handle additions (purchases), removals (sales), or deaths with options to preserve or delete history.  
- **Excel export:** generate a spreadsheet with key animal information for reports and administration.  
- **User-friendly interface:** simple navigation and minimal required fields, designed for non-technical users.

---

## 🧩 Requirements

- **Java JDK 8 or later** (LTS recommended).  
- **IDE** such as Eclipse, IntelliJ IDEA, or VS Code with Java extension, or CLI tools (`javac`, `java`).  
- **External libraries** included in the `lib/` directory (e.g., Excel handling).

---

## ⚙️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/JPehaDev/Data-_Base_Livestock.git
   cd Data-_Base_Livestock
   ```

2. **Open in your IDE**
   - Import as an **Eclipse project** (metadata files like `.project` and `.classpath` are available).
   - Or configure with **Maven/Gradle** if you plan to modernize the build (see [Roadmap](#-roadmap)).

3. **Configure dependencies**
   - Ensure that all JARs in the `lib/` folder are included in the classpath.
   - Verify that the **JRE System Library** points to your installed JDK.

4. **Compile and run**
   - In your IDE, run the class containing the `main` method (e.g., `Main`).
   - Or from the console:
     ```bash
     javac -cp "lib/*:src" -d bin src/**/*.java
     java -cp "lib/*:bin" Main
     ```
     > Replace `Main` with the actual class name. On Windows, use `;` instead of `:` as the path separator.

---

## ▶️ Usage

1. **Choose the operation**: query, inventory, purchase/sale, or loss.  
2. **Register or edit animals** with their details (ID, sex, weight, breed/color).  
3. **Search** an animal by its number to view its record.  
4. **Export to Excel** to generate reports and backups.

---

## 🗂️ Project Structure

```
Data-_Base_Livestock/
├─ .settings/        # IDE metadata (Eclipse)
├─ bin/              # Compiled classes (output)
├─ lib/              # External dependencies (e.g., Excel libraries)
├─ src/              # Java source code (UI, logic, Excel export)
├─ LICENSE           # EPL-2.0 license
└─ README.md
```

---

## 🧭 Roadmap

- [ ] Migrate to **Maven/Gradle** for modern dependency management.  
- [ ] Add **JUnit tests** for business logic.  
- [ ] Internationalization (Spanish/English).  
- [ ] Enhanced validations (weight ranges, breed catalogs).  
- [ ] Standardized Excel templates and dashboard support.  
- [ ] Optional persistence with **SQLite/PostgreSQL** in addition to Excel.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repo.  
2. Create a branch: `git checkout -b feature/new-feature`.  
3. Commit your changes with clear messages.  
4. Open a Pull Request describing your changes and test steps.

---

## 📄 License

This project is licensed under the **EPL-2.0 (Eclipse Public License v2.0)**. See the `LICENSE` file for details.

---

## 🙌 Credits

- Original project: **Base-de-Datos-con-Excel-MACC**.  
- Fork and adaptation: **@JPehaDev**.

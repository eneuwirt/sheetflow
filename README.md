# SheetFlow

**SheetFlow** is a modular platform for comparing, analyzing, and transforming structured Excel files. Designed for technical and financial domains, it enables rule-based workflows for documents such as cost breakdown sheets, pricing tables, and technical evaluations.

---

## 🔧 Architecture Overview

The project is divided into three main components:

- **🧠 TableLogic (Core)**  
  The core engine responsible for structural analysis, comparison logic, and a domain-specific language (DSL) for defining rules

- **🖥️ SheetFlow App (Web)**  
  A modern Vaadin 24 + Spring Boot web application for managing users, projects, file uploads, and visualizing comparison results

- **💻 TableLogic CLI**  
  A command-line interface to run comparisons outside the GUI, e.g., for CI/CD or scripting scenarios

---

## 📁 Project Structure
sheetflow/
├── tablelogic-core/ # Core comparison logic, DSL, structural parsing
├── tablelogic-cli/ # CLI tool for automated comparisons
├── sheetflow-app/ # Web UI, user and project management
└── README.md # This file

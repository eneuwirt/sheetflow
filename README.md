# SheetFlow

**SheetFlow** is a web-based platform for comparing and processing structurally similar Excel files.  
It is built with Java, Spring Boot, and Vaadin, and supports multiple users, PostgreSQL integration, and Docker deployment.

The core logic is handled by a custom domain-specific language (DSL) named **TableLogic**, which defines comparison and transformation rules for tabular data.  
TableLogic is integrated into SheetFlow and also available as a standalone CLI tool.

---

## Project Structure

- `com.sheetflow` – Main web application (Vaadin + Spring Boot)
- `tablelogic-core` – DSL engine (comparison logic, rule evaluation)
- `tablelogic-cli` – Standalone CLI wrapper for `tablelogic-core`
- `sheetflow-db` – PostgreSQL schema and migration scripts
- `docker/` – Docker setup for local and production use

---

## Key Features

- Rule-based comparison of Excel files (with support for tolerances, mappings, conditions)
- DSL definition of transformation and comparison logic (`TableLogic`)
- Multi-user project structure
- Storage of Excel data and files in PostgreSQL
- CLI and WebApp support
- Clean modular architecture (separation of logic, UI, storage)

---

## Technology Stack

- Java 21
- Spring Boot
- Vaadin 24
- PostgreSQL
- Docker
- Maven

---

## Getting Started

To build and run locally:

```bash
git clone https://github.com/your-org/sheetflow.git
cd sheetflow
docker compose up --build

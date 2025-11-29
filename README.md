# SG Technologies POS System

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=ShajiaT_pos_system&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=ShajiaT_pos_system)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=ShajiaT_pos_system&metric=bugs)](https://sonarcloud.io/summary/new_code?id=ShajiaT_pos_system)
[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=ShajiaT_pos_system&metric=code_smells)](https://sonarcloud.io/summary/new_code?id=ShajiaT_pos_system)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=ShajiaT_pos_system&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=ShajiaT_pos_system)

## Overview

This is a legacy Point-of-Sale System developed for CSE216 Software Engineering course (Alpha Release - December 9, 2015). This repository is part of a Software Reengineering project to analyze, document, and modernize the existing codebase.

**Current Status:** Under analysis and reengineering

## Project Information

- **Original Release:** Alpha Release - Dec 9, 2015
- **Course:** CSE216 - Software Engineering
- **Organization:** SG Technologies
- **Purpose:** Educational project demonstrating POS system with sales, rentals, and returns functionality

## Features

- Employee authentication (Admin/Cashier roles)
- Sales transactions with tax calculation
- Rental management with due date tracking
- Return processing
- Coupon/discount support
- Employee management (CRUD operations)
- Inventory tracking
- Transaction logging

## Technology Stack

- **Language:** Java 8
- **GUI Framework:** Swing
- **Build Tool:** Apache Ant
- **Data Storage:** Text files (pseudo-database)
- **Design Patterns:** Singleton, Abstract Factory
- **Testing:** JUnit 4

## Quick Start

### Prerequisites
- JDK 8 or higher
- Apache Ant (or NetBeans IDE)

### Compilation

Using Ant:
```bash
ant compile
```

Using javac:
```bash
mkdir -p bin
javac -d bin src/*.java
```

### Running the Application

```bash
java -cp bin Register
```

**Default Login Credentials:**
- Admin: Username: `110001`, Password: `1`
- Cashier: Username: `110002`, Password: `lehigh2016`

## Project Structure

```
.
├── src/                    # Source code files
├── tests/                  # JUnit test files
├── Database/              # Text file data storage
├── Documentation/         # Project documentation
├── nbproject/            # NetBeans project files
├── build.xml             # Ant build script
└── README.md             # This file
```

## Design Patterns

- **Singleton Pattern:** `Inventory.java` - Ensures single inventory instance
- **Abstract Factory Pattern:** `PointOfSale.java` - Base class for POS, POR, POH transactions

## Known Issues & Limitations

⚠️ This is a legacy educational project with the following limitations:

- Text file-based storage (no actual database)
- Plain text password storage
- Single-user desktop application
- No concurrent access control
- Minimal test coverage
- Mixed architectural concerns

**See [INVENTORY_ANALYSIS_REPORT.md](INVENTORY_ANALYSIS_REPORT.md) for detailed analysis.**

## Reengineering Roadmap

This project is undergoing software reengineering as part of an academic project. See the comprehensive inventory analysis report for:

- Complete asset inventory
- Dependency mapping
- Architecture assessment
- Security vulnerabilities
- Modernization recommendations

## SonarQube Analysis

This project uses SonarCloud for continuous code quality monitoring. Analysis runs automatically on every push to the main branch.

**View Results:** [SonarCloud Dashboard](https://sonarcloud.io/project/overview?id=ShajiaT_pos_system)

## Documentation

- [Original README](README.txt) - Original project documentation
- [Inventory Analysis Report](INVENTORY_ANALYSIS_REPORT.md) - Comprehensive reengineering analysis
- [Documentation Folder](Documentation/) - Phase-wise project documentation

## Contributors

**Original Development Team (2015):**
- CSE216 Software Engineering Students

**Reengineering Analysis (2025):**
- ShajiaT

## License

Educational project - No specific license

## Contact

For questions about the reengineering analysis, please refer to the course materials or contact the project maintainer.

---

**Note:** This is a legacy system being analyzed for educational purposes. It is not recommended for production use without significant refactoring and modernization.

# CS 320: Software Test Automation and Quality Assurance Portfolio

## Project Overview
This repository contains key artifacts from CS 320 (Software Test Automation & QA). It highlights back-end unit testing using JUnit 5 and JaCoCo code coverage, alongside a comprehensive reflections report on software quality and testing methodologies.

---

## Portfolio Reflections

### How can I ensure that my code, program, or software is functional and secure?
Ensuring functionality and security requires a multi-layered testing strategy combining both automated unit testing and defensive programming practices. To guarantee functionality, I utilize automated frameworks like JUnit 5 to test both positive execution flows ("happy paths") and edge-case boundary conditions. Achieving 100% line and branch coverage ensures that every branch of execution and condition is evaluated. Security is embedded by enforcing strict input validation and immutability within domain models—rejecting null values, out-of-bound string lengths, and improper parameter formats before they reach service logic or persistence layers. Additionally, incorporating exception handling (such as `assertThrows`) ensures the system safely fails without exposing sensitive internal states.

### How do I interpret user needs and incorporate them into a program?
Interpreting user needs begins with carefully analyzing functional and non-functional software requirements and translating them into technical constraints. I map user requirements directly into verifiable unit tests before writing operational code (adopting a Test-Driven Development approach where appropriate). For example, if business requirements mandate that a contact ID must be non-null and no longer than 10 characters, I create automated test cases that explicitly validate those rules. This ensures that every software feature directly corresponds to customer expectations while guaranteeing that requirements are automatically enforced throughout the software lifecycle.

### How do I approach designing software?
My approach to software design is rooted in modularity, encapsulation, and maintainability. I prioritize object-oriented principles, separating entity models (e.g., `Contact`, `Task`, `Appointment`) from service logic (e.g., `ContactService`) to ensure clear separation of concerns. Designing software with testability in mind from day one leads to cleaner, loosely coupled architectures that utilize in-memory data structures or interfaces for rapid feedback. Furthermore, I approach software design with a focus on long-term quality, avoiding technical debt by writing comprehensive test suites, enforcing strict boundary checks, and using continuous integration practices to ensure stability across future updates.

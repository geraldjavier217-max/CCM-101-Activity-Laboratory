# Two-Tier Architecture

## Introduction
A two-tier architecture is an application design that separates a system into two main parts: the web/application tier and the database tier. These tiers communicate with each other to provide the application's services.

## The Web/Application Tier
The web/application tier handles user requests and displays the application's interface through a web browser. In this project, Nextcloud serves as the web application that allows users to access and manage their files through a browser.

## The Database Tier
The database tier stores and manages persistent information, including user account details, file metadata, and application settings. In this project, MariaDB serves as the database for Nextcloud.

## Why Separate Them?
Separating the web application and database into different containers makes the system easier to manage, update, and troubleshoot. It also allows each service to be configured and scaled independently while keeping database services separate from direct browser access.

## Architecture Diagram

```text
+------------------------+
|     User's Browser     |
+-----------+------------+
            |
            | HTTP (Port 8080)
            v
+------------------------+
| Nextcloud Application  |
|     Web Tier           |
+-----------+------------+
            |
            | Database Connection
            v
+------------------------+
|       MariaDB          |
|     Database Tier      |
+------------------------+
```

## Conclusion
The two-tier architecture provides a clear separation between application processing and data storage. Docker Compose helps deploy and manage both containers as one application stack.

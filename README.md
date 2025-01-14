# INFORCE .NET TASK - URL Shortener

## Overview

This project implements a **URL Shortener** application with ASP.NET MVC, Angular, and Entity Framework. The application allows users to shorten URLs, navigate using the shortened equivalents, and manage URLs with detailed access control based on user roles (Admin, Authorized User, and Anonymous User).

---

## Features

### 1. **Login View**
- Users can log in with their credentials (Login, Password).
- Supports two roles: 
  - **Admin**: Full access to all records and administrative capabilities.
  - **Authorized User**: Limited access to records created by the user.
- Authorization is required to perform sensitive actions.

### 2. **Short URLs Table View**
- Displays a table of all shortened URLs and their original counterparts.
- Features:
  - Add new URL (only for authorized users).
  - Delete URLs:
    - Admin users can delete any URL.
    - Authorized users can delete their own URLs.
  - Real-time updates to the table without page reloads (Angular integration).
  - Navigate to detailed URL info using the Short URL Info view.

- **Validation:**
  - URLs must be unique.
  - If a URL already exists, an error message is displayed.

### 3. **Short URL Info View**
- Displays detailed information about a URL:
  - Created By
  - Created Date
  - Additional metadata.
- Access restricted to authorized and admin users.

### 4. **About View**
- A descriptive page explaining the URL shortening algorithm.
- Publicly accessible to all users.
- Editable by Admin users.

---

## Technical Stack

- **ASP.NET MVC** (Framework or Core)
- **Angular** (Latest version)
- **Entity Framework Code-First** for database management
- **Unit Testing Framework** (e.g., xUnit, NUnit, MSTest)

# 📚 Library Management System – Database Design (ERD)

## Overview & Objectives

This assignment is designed to help beginners understand database design concepts using a **Library Management System**.

By completing this assignment, you will be able to:

- Design an ERD with **1 to 1**, **1 to Many**, and **Many to 1** relationships
- Identify **primary keys (PK)** and **foreign keys (FK)**
- Understand how real-world library operations are converted into database tables

---

## Database Design & Business Logic

The Library Management System manages:

- **Members**
- **Books**
- **Borrowings**

### Business Logic – What Your Database Must Handle

Your database design should support the following real-world scenarios:

#### Members Table Must Store:

- Member role _(Admin / Student / General Member)_
- Full name
- Email address _(must be unique)_
- Phone number
- Membership date
- Account status _(active / inactive)_

#### Books Table Must Store:

- Book title
- Author name
- Book category _(e.g., Fiction, Science, History)_
- ISBN number _(must be unique)_
- Total copies
- Available copies
- Book status _(available / not available)_

#### Borrowings Table Must Store:

- Which member borrowed the book _(link to Members table)_
- Which book was borrowed _(link to Books table)_
- Borrow date
- Due date
- Return date _(can be NULL if not returned)_
- Borrowing status _(borrowed / returned / overdue)_

---

## ERD Design

Design an **Entity Relationship Diagram (ERD)** for the Library Management System.

### Required Tables

Your ERD must include the following tables:

- **Members**
- **Books**
- **Borrowings**

### Relationship Requirements

Your ERD must clearly show:

#### One to Many:
- One Member → Many Borrowings

#### Many to One:
- Many Borrowings → One Book

#### One to One (logical):
- Each borrowing record connects exactly one member and one book

### ERD Must Include:

- ✅ Primary Keys (PK)
- ✅ Foreign Keys (FK)
- ✅ Proper relationship cardinality
- ✅ Status fields (member status, book status, borrowing status)

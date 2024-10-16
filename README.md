# Code First Approach with Entity Framework Core

This project demonstrates how to implement the Code First approach using Entity Framework Core to create a database and relationships.

## Overview

In this project, two tables are created:
1. **User Table**
2. **Post Table**

Each user can have multiple posts, but each post belongs to a single user.

### User Table
- `Id` (int): Primary key and auto-incremented.
- `Username` (string): The username of the user.
- `Email` (string): The email address of the user.

### Post Table
- `Id` (int): Primary key and auto-incremented.
- `Title` (string): The title of the post.
- `Content` (string): The content of the post.
- `UserId` (int): Foreign key, representing the user who authored the post.

### Relationships
- A user can have many posts, but a post is authored by only one user.

## Database Context

The database context class is named `PatikaSecondDbContext`. This class handles interactions with the database.

### Database Name
The database name for this project is **PatikaCodeFirstDb2**.

### Tables
The database contains two tables:
- **Users**
- **Posts**

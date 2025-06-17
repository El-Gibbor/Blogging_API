# Blog API

A RESTful API for a blogging platform built with Node.js, MongoDB, and Passport.js. It supports user authentication, blog creation, management, and discovery.

---
## Features

### 1. User Authentication
- Sign up with `first_name`, `last_name`, `email`, and `password`
- Sign in with `email` and `password`
- Authentication handled with Passport + JWT (token expires in 1 hour)

### 2. Blog Access
- All users (logged in or not) can:
  - View a paginated list of published blogs
  - View individual published blog posts (read count increases automatically)
- Blogs are searchable by author, title, and tags
- Blogs are sortable by `read_count`, `reading_time`, or `timestamp`

### 3. Blog Management
- Blogs can be in either `draft` or `published` state
- Authenticated users can:
  - Create blogs (default state: `draft`)
  - Publish/unpublish their blogs
  - Edit or delete their blogs
  - View their blogs (filterable by state)

### 4. Blog Schema
Each blog includes:
- `title`, `description`, `tags`, `author`, `timestamp`
- `state`, `read_count`, `reading_time`, `body`

---

## Getting Started

### Prerequisites
- Node.js
- MongoDB Atlas (or local MongoDB)

### Setup

```bash
# Clone the repository
git clone https://github.com/El-Gibbor/Blogging_API.git

# Navigate into the project folder
cd Blogging_API

# Install dependencies
npm install

# Run the server
node index.js
```

## API Base Url:
https://api-blog-m07l.onrender.com


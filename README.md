# Contact Form Project

This project includes a simple contact form that allows users to submit their name, email, and message. The submitted data is then stored in a MySQL database.

## Setup Instructions

1. **Database Setup:**

   - Execute the following SQL script in your MySQL environment to set up the required database and table:

   ```sql
   -- Create the database if it doesn't exist
   CREATE DATABASE IF NOT EXISTS your_database;

   -- Switch to the specified database
   USE your_database;

   -- Create the 'form_data' table if it doesn't exist
   CREATE TABLE IF NOT EXISTS form_data (
       id INT AUTO_INCREMENT PRIMARY KEY,
       name VARCHAR(255) NOT NULL,
       email VARCHAR(255) NOT NULL,
       message TEXT NOT NULL,
       created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
   );
   ```

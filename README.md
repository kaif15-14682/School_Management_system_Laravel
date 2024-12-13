# How to Run the Project

Follow these instructions to set up and run the project on your local machine:

## Prerequisites
Before proceeding, ensure you have the following installed:
- **PHP** (Recommended: version 8.0 or later)
- **Composer**
- **MySQL**
- **A web server** (e.g., Apache or Nginx)
- **A terminal or command-line interface**

## Steps to Run the Project

1. **Download and Extract the Project**
   - After downloading the project, unzip the project file into a directory of your choice.

2. **Update the Environment Configuration**
   - Open the project folder.
   - Locate the `.env` file (or create one by copying the `.env.example` file).
   - Update the database credentials in the `.env` file, such as `DB_DATABASE`, `DB_USERNAME`, and `DB_PASSWORD`, to match your local setup.

3. **Create the Database**
   - Open your MySQL interface (e.g., phpMyAdmin or MySQL Workbench).
   - Create a new database using the name specified in the `.env` file.

4. **Install Dependencies**
   - Open a terminal or command prompt and navigate to the project folder.
   - Run the following command to install the required Composer dependencies:
     ```bash
     composer install
     ```

5. **Migrate the Database**
   - Run the following command to create the necessary tables in your database:
     ```bash
     php artisan migrate
     ```

6. **Seed the Database**
   - Populate the database with initial data using this command:
     ```bash
     php artisan db:seed
     ```

7. **Serve the Application**
   - Start the Laravel development server using the following command:
     ```bash
     php artisan serve
     ```
   - The server will start, and a URL (e.g., `http://127.0.0.1:8000`) will be provided in the terminal.

8. **Access the Application**
   - Open the provided URL in your favorite browser. We recommend using Google Chrome for the best experience.

9. **Login Credentials**
   For admin portal login:
   username: admin@gmail.com
   pass: 1234
   For student portal login:
   username: student@gmail.com
   pass: 1234
   For teacher portal login:
   username: teacher@gmail.com
   pass: 1234
   For Parents portal Login:
   username: parent@gmail.com
   pass:1234
   *You can always change and set the username and password from the database*

## Notes
- If you encounter issues, ensure that your PHP and MySQL services are running.
- If changes do not reflect, clear the application cache using:
  ```bash
  php artisan cache:clear
  php artisan config:clear
  php artisan view:clear
  ```

Enjoy using the project!


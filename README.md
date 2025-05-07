# SportsStore ASP.NET Setup Guide (with MySQL via XAMPP)

##  1. Extract the Project

- Download the ZIP from GitHub.
- Extract it and open the folder in your ASP.NET IDE (e.g., Visual Studio).

##  2. Setup MySQL with XAMPP

- Open XAMPP and start **Apache** and **MySQL**.
- Go to [http://localhost/phpmyadmin](http://localhost/phpmyadmin).
- Create a new database named `sportsstore`.
- Import `sportsstore.sql` using the **Import** tab.

##  3. Configure ASP.NET Connection

- Open your `appsettings.json` or wherever your connection string is stored.
- Update it like this:

```json
"ConnectionStrings": {
  "DefaultConnection": "server=localhost;user=root;password=;database=sportsstore;"
}

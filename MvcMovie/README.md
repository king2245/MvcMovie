# MvcMovie — Movie Management Application

## 1. Get Started
This project is a movie management web application developed using ASP.NET Core MVC in Visual Studio.

## 2. Create the Project
The MvcMovie project was created in Visual Studio using the ASP.NET Core MVC template.

## 3. Add a Model
The `Movie` model represents a movie and contains properties such as `Id`, `Title`, `Genre`, `Price`, and `ReleaseDate`.

## 4. Add a Database Context
The `MovieDbContext` class connects the movie model to the database using Entity Framework Core.

## 5. Configure the Database
The application uses SQL Server LocalDB. The database connection string is configured in `appsettings.json`.

## 6. Add a Controller
The `MoviesController` handles requests related to listing, creating, editing, and deleting movies.

## 7. Add Views
Razor views provide the interface for displaying the movie list and the Create, Edit, and Delete pages.

## 8. Add Database Migrations
Entity Framework Core migrations record database schema changes and help create or update the database.

## 9. Implement CRUD Operations
The application supports:
- **Create:** Add a new movie.
- **Read:** View the list of movies.
- **Update:** Edit movie details.
- **Delete:** Remove a movie after confirmation.

## 10. Run and Test the Application
1. Open `MvcMovie.slnx` in Visual Studio.
2. Restore NuGet packages if prompted.
3. Ensure SQL Server LocalDB is installed.
4. Run the application using the HTTPS launch profile.
5. Test creating, viewing, editing, and deleting movies.

## Technologies Used
- C#
- ASP.NET Core MVC
- Entity Framework Core
- Razor Views
- SQL Server LocalDB
- Git and GitHub
## Detailed Testing Checklist

- [ ] Create a new movie and save it.
- [ ] Confirm the movie appears in the movie list.
- [ ] Open the Edit page and change the movie details.
- [ ] Confirm the changes are saved.
- [ ] Open the Delete page for a movie.
- [ ] Confirm deletion and verify the movie is removed.
- [ ] Check that the application displays validation errors for invalid input.
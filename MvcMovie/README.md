# MvcMovie – Movie Management Application

## 1. Get Started

This is my movie management application, which I developed using ASP.NET Core MVC in Visual Studio. I built it to practise creating a web application that can store and manage movie information.

Users can add movies, view the list of movies, edit their details, and delete movies they no longer need.

## 2. Create the Project

I created the `MvcMovie` project in Visual Studio using the ASP.NET Core Web App (Model-View-Controller) template.

After creating the project, I checked that it could run before adding the movie management features. This helped me make sure the basic application was working correctly.

## 3. Add a Model

I created a `Movie` model in the `Models` folder. This class describes the information I want to save for each movie.

The model contains these properties:

- `Id` – identifies each movie.
- `Title` – stores the movie's title.
- `Genre` – stores the type or category of the movie.
- `Price` – stores the movie's price.
- `ReleaseDate` – stores the date the movie was released.

## 4. Add a Database Context

I added a `MovieDbContext` class in the `Data` folder. It connects my movie model to the database through Entity Framework Core.

The context allows the application to work with movie records without writing every database operation manually.

## 5. Configure the Database

I configured the database connection in `appsettings.json`. My project uses SQL Server LocalDB to store movie information.

The connection string tells the application which database to use. The database must be available on the computer where the project is running.

## 6. Add a Controller

I created a `MoviesController` to handle requests from the movie pages.

The controller works with `MovieDbContext` to retrieve movie records and save changes. It handles the main actions needed to create, display, edit, and delete movies.

## 7. Add Views

I added Razor views in the `Views/Movies` folder to provide the pages users interact with.

- `Index.cshtml` displays the list of movies.
- `Create.cshtml` contains the form for adding a movie.
- `Edit.cshtml` allows a user to change a movie's details.
- `Delete.cshtml` asks the user to confirm before deleting a movie.

These pages make it possible to manage movie records through the browser.

## 8. Add Database Migrations

I used Entity Framework Core migrations to keep track of changes to the database structure.

The project contains migration files that describe the database changes made during development. These migrations help create or update the database to match the model.

## 9. Implement CRUD Operations

After connecting the model, database, controller, and views, I tested the main features of the application.

- **Create:** I can add a new movie.
- **Read:** I can view the saved movies in a list.
- **Update:** I can edit the details of an existing movie.
- **Delete:** I can remove a movie after confirming the deletion.

These are the main features of my movie management application.

## 10. Run and Test the Application

To run the project, I open `MvcMovie.sln` in Visual Studio and start the application using the HTTPS launch profile.

I tested the application by:

1. Adding a new movie and saving it.
2. Checking that the movie appeared in the list.
3. Editing the movie's details and saving the changes.
4. Deleting the movie and checking that it was removed.
5. Checking how the application responds to invalid input.

The database must be configured correctly, and SQL Server LocalDB must be available for the application to save its data.

## Technologies Used

- C#
- ASP.NET Core MVC
- Entity Framework Core
- Razor Views
- SQL Server LocalDB
- Git and GitHub

## Testing Checklist

- [ ] Add a new movie.
- [ ] Check that it appears in the list.
- [ ] Edit the movie and save the changes.
- [ ] Confirm that the updated details appear.
- [ ] Delete the movie.
- [ ] Check that it no longer appears in the list.
- [ ] Test invalid input and check for validation messages.

## GitHub Repository

My project is available on GitHub:

https://github.com/king2245/MvcMovie
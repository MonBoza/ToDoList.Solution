# To Do List

## To do list web app

### By Monica Barboza

## Technologies Used

* C#
* ASP.NET

## Description

## Setup/Installation Requirements

* Open terminal or command prompt.
* Clone the repository by running the following command to your desktop: git clone <https://github.com/MonBoza/ToDoList.Solution.git>
* Make sure .gitignore is added to repository.
* Run `dotnet build` in your terminal
* Run test by navigating to the test directory and running `dotnet restore` and then `dotnet test`
* Tests are located in Project.Test directory.
* Open the project in your favorite code editor.

## Known Bugs

* _Any known issues_
* _should go here_

## License

Copyright 2024 MONICA BARBOZA

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

Email: (mailto:<MonBoza@gmail.com>)

Copyright (c) Month day, 2024 Monica Barboza


What Is This?
This is an example repo corresponding to multiple lessons within the LearnHowToProgram.com walkthrough on creating a To Do List application in Section 4: Many-to-Many Relationships.

This project corresponds to the classwork and lessons that describe how to connect an ASP.NET Core MVC project to a MySQL database using Entity Framework Core with migrations. This project contains a one-to-many relationship between Item and Category, and a many-to-many relationship between Item and Tag. There are multiple lessons in this series. The first lesson in the series is Code First Development and Migrations.

There are multiple branches in this repo that are described more below.

How To Run This Project
Install Tools
Install the tools that are introduced in this series of lessons on LearnHowToProgram.com.

Set Up and Run Project
Clone this repo.
Open the terminal and navigate to this project's production directory called "ToDoList".
Within the production directory "ToDoList", create a new file called appsettings.json.
Within appsettings.json, put in the following code, replacing the uid and pwd values with your own username and password for MySQL. For the LearnHowToProgram.com lessons, we always assume the uid is root and the pwd is epicodus.
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=to_do_list_with_many_to_many;uid=root;pwd=epicodus;"
  }
}
Create the database using the migrations in the To Do List project. Open your shell (e.g., Terminal or GitBash) to the production directory "ToDoList", and run dotnet ef database update.
To optionally create a migration, run the command dotnet ef migrations add MigrationName where MigrationName is your custom name for the migration in UpperCamelCase. To learn more about migrations, visit the LHTP lesson Code First Development and Migrations.
Within the production directory "ToDoList", run dotnet watch run in the command line to start the project in development mode with a watcher.
Open the browser to https://localhost:5001. If you cannot access localhost:5001 it is likely because you have not configured a .NET developer security certificate for HTTPS. To learn about this, review this lesson: Redirecting to HTTPS and Issuing a Security Certificate.
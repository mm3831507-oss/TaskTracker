# TaskTracker

A simple task management web app built with C#, Blazor, .NET 10, and SQLite.

## Purpose

TaskTracker helps users organize daily tasks and track unfinished work.
Users can add, edit, complete, and delete tasks through a simple web interface.
Tasks remain saved after the application restarts.

## Features

- Add new tasks.
- Edit existing tasks.
- Mark tasks as complete or incomplete.
- Delete tasks.
- View the remaining-task count.
- Save tasks in SQLite so they remain after restarting the app.
- Reject empty task names when adding or editing.
- View instructions on the About page.

## Requirements

- Visual Studio 2026 with the ASP.NET and web development workload.
- .NET 10 SDK.

## How to Run

1. Open TaskTracker.slnx in Visual Studio.
2. Allow NuGet packages to restore.
3. Select the https launch profile.
4. Press F5 to start the app.
5. Use the task page in the browser.

## How to Use

- Enter a task name and click Add Task.
- Click Edit to update a task name, then click Save.
- Click Cancel to discard an edit.
- Use the checkbox to change a task's completion status.
- Click Delete to remove a task.
- Click About to view the application instructions.

## Manual Testing

The following checks passed during manual testing:

- Add a task and update the remaining-task count.
- Edit and save a task name.
- Mark a task complete and incomplete.
- Delete a task.
- Keep an added task after restarting the application.
- Reject empty task names when adding or editing.
- Cancel an edit without changing the saved task.
- Display the layout and open the menu in a narrow browser window.
- Open About and return using Back to tasks.

## Data Storage

Tasks are stored locally in App_Data/tasks.db using SQLite.
The application automatically creates the folder, database,
and Tasks table on first run. No separate database setup is required.

Task names and completion status are stored in the database.

## Author

Manoj Mandal
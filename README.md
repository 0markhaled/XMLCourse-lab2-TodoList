# XMLCourse-lab2-TodoList

1)created the prject by running the terminal command
dotnet new webapi  -o "filename"


added thse packages
dotnet add package Microsoft.EntityFrameWorkCore.InMemory //this is used for storing the POST requests in memeory incase there is no DB
dotnet add package Microsoft.EntityFrameWork.sqserver
dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design
dotnet add package Microsoft.EntityFrameworkCore.Design
dotnet add package Microsoft.EntityFrameworkCore.Tools     // allows us to use the asp generator tool which creates the controller

 aspcode generator used to create controller
 dotnet aspnet-codegenerator controller -name TodoItemsController -async -api -m TodoItem -dc TodoContext -outDir Controllers
 
 this app uses an API controller such as Postman to ceate Get/Post requests. 
 
 the project was modified so it allows the us to extratct the data in XML in addition to the default Json
 
 COnnection String was made to allows us to use Sqlite as db.
 
 The app lists the tasks added via postman POST request, on the console and html <ul> in th browswer.
 
 It displays in the console and broswer via simple html dynamically.
 
 *****To use this app, run the server.
 
 Swagger will automaitcally open, 
 use the POST method to add to the do to list.
 
 than navigate to the localhost server/index.html and the to do list should appear there
 

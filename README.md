# EvolentContactProject
Project uploaded for evolent

Installation instructions:
1. Download EvolentContactProject.zip and unzip the folder EvolentContactProject-main.zip and all the folders inside it.
2. Copy folder EntityFramework.6.1.3 and EntityFramework.6.4.0 in folder EmployeeData\packages
3. Copy all the folders from packages1 in folder EmployeeData\packages
4. Import bacpac file from folder DatabaseFiles in SSMS. This will import required database and table.
5. Open visual studio and open EmployeeData.sln from folder EmployeeData
6. Add DataAccess project from folder DataAccessLayer in visual studio
7. Add EmployeeDataConsumeWebApi project in visual studio and mark this project as startup project.
8. If there is any issue in reference add dll'd directly from DLL folder
9. If there is any issue in Global.asax.cs file then execute below nuget command in package manager console
Update-Package Microsoft.AspNet.WebApi.WebHost -reinstall

Folders Use:
1. Following folders are available in this project : DataAccessLayer,EmployeeData,EmployeeDataConsumeWebApi & DatabaseFiles.
2. DataAccessLayer : DAL.cs class in this project is used to access the data from DB by Web API service
3. EmployeeData : WEB API project
4. EmployeeDataConsumeWebApi : ASP.NET MVC application which consumes EmployeeData web api service.
5. DatabaseFiles : It contains bacpac file(Import this file in SSMS)

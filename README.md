# Pierre's Sweet and Savory Treats 

#### This is a C# application for a bakery owner

#### By Mary Marks

## Technologies Used

- .NET Core 5.0.1
- ASP.NET Core MVC
- ASP.NET Core Razor Pages
- C#
- Entity Framework Core
- GitHub
- HTML
- MySQL
- MySQL Workbench
- VS Code

## Description

This is a C#/.NET treat and flavor tracker app for a bakery demonstarating many to many relationships. It allows the user to input new treats and flavors. The user can view a list of all treats and flavors and add flavors to treats. Only authorized users can edit information.

## Setup/Installation Requirements

##### Software Requirements

1. Internet browser
2. A code editor such as VSCode to view and edit the code
3. .NET or follow along with the Installing .NET instructions to install .NET

##### Open Locally

- Click on the link to my repository: [https://github.com/maryleemarks/PierresTreats.Solution]()
- Click on the green "Code" button and copy the repository URL
- Open your terminal and use the command `git clone https://github.com/maryleemarks/PierresTreats.Solution` into the directory you would like to clone the repository
- Open in text editor to view code and make changes

##### Installing .NET

In order to run the application, please install .NET for your computer to recognize the `dotnet` command.

1. Download [.NET Core SDK (Software Development Kit)](https://dotnet.microsoft.com/download/dotnet). Clicking this link will prompt a file download for your particular OS from Microsoft.
2. Open the file. Follow the installation steps.
3. Confirm the installation is successful by opening your terminal and running the command `dotnet --version`. The response should be something similar to this:`5.0.100`. This means it was successfully installed.

##### Installing MySQL

MySQL is a type of database software used to create, edit, query, and manage SQL data.

- For Mac Users please [Click Here](https://dev.mysql.com/downloads/file/?id=484914) to download MySQL Installer
- For Windows Users please [Click Here](https://dev.mysql.com/downloads/file/?id=484919)

- Verify MySQL installation by opening the terminal and entering the command `mysql -uroot -p[THEPASSWORDYOUSELECTED]`
- If you gain access you will see see the MYSQL command line!

##### Installing MySQL Workbench

- Please [Click Here](https://dev.mysql.com/downloads/workbench/) to install the correct version for your machine
- Open MySQL Workbench and select `Local instance 3306 server`. You will need to enter the password you selected

##### Compiling

- Navigate to the PierresTreats folder in the command line
- Use the command `dotnet build` to compile

##### Installing Packages

- Navigate to the PierresTreats folder in the command line
- Use the command `dotnet restore`

<details>

  <summary>Expand for Database Installation Essentials!</summary>

### Database Connection

Create a connection string to connect the database to the web application

1. Create a file in the root directory called `appsettings.json`
2. Add the code below:

```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=[YOUR-DATABASE-NAME-HERE];uid=[YOUR-USERNAME-HERE];pwd=[YOUR-PASSWORD-HERE];"
  }
}
```

- Update all the information above in the square brackets. Change the server, port, and uid if necessary.

### Import/Update Database Using Entity Framework Core

- Navigate to `PierresTreats` directory in terminal
- Use the command `dotnet ef database update` to update the database migration through Entity Framework Core


### Update Database Using MySQL Workbench

1. Open MySQL Workbench
2. Click on Server > Data Import in the top navigation bar
3. Select `Import from Self-Contained File`
4. Select the `Default Target Schema` or create new schema
5. Select all Schema Objects you would like to import
6. Select `Dump Structure and Data`
7. Click `Start Import`

</details>

##### View In Browser

- To view in browser, navigate to PierresTreats folder in the command line
- Use the command `dotnet run` to execute the compiled code and start a localhost
- In browser navigate to http://localhost:5000

## Known Bugs

* None

## License

MIT

## Contact Information

* Mary Marks <maryleemarks@gmail.com>

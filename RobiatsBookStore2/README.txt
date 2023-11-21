2023-10-23 12:38
 A 5.0.NET Application was created for the assignment 2
 i enabled the individual account under the authentication while creating this new project

 12:40
 i went to my launchSettings.json under my properties and comment out //"sslPort": 44321 to enable me have access to my web page

 12:42
 I created a README.txt file to add details about my project

 12:45
 i went to my startup.cs AND TOOK THIS OUT //options => options.SignIn.RequireConfirmedAccount = true

 2023-10-24 2:36
 i updated the database using the Update-Database in the management console

 2:37
 I went through the vires and data folder to get familiar with the files and the contents in it 

 3:10 
 I downloaded the bootstap file and added it to my css folder i already have a bootstap.cs file in my css so instead of deleting it i renamed 
 incase the one i downloaded didnt work i will have that as my backup

 3:13
 i went to my layout.cshtml and i linked the bookstap i downloaded while commenting out the one i have there previously

 3:32
 i also changed the nav class from the navbar-light to navbar-dark and bg-white to bg-primary

 3:36
 i made some changes in my footer in te renderbody function and added some properties which is the text-white-50 bg-primary

 3:39
 in my loginPartial.cshtml i removed the references to text-dark

 2023-10-30 11:35
 I started my project by cleaning and building the project again and everything is working perfectly

 11:42
 in my layout.cshtml page i added the additionL stylesheet and scriptfrom the CSS_LS file provided for us

 11:55
 in my layout.cshtml page i added the additionL stylesheet and scriptfrom the CSS_LS file provided for us

 1:19
 IN MY SHARED LAYOUT.CSHTML FILE I ADDED A DROP DOWN NAVIGATION MENU IMMEDIATELY AFTER MY PRIVACY LINK

 1:28
 i changed this display text from dropdown to content management

 1:29
 I created a new project in my class library i created three new projects in my solution folder
 RobiatsBooksStore.DataAccess,
 RobiatsBooksStore.Models,
 RobiatsBooksStore.Utility
 I copied my data folder in my project and pasted it in my  RobiatsBooksStore.DataAccess and deleted the original data folder from my project

 2:16
 I installed the Microsoft.EntityFrameWork Core.Relational and thhe Core.sqlServer packages 
 successfully installed

 2:18
 I DELETED THE MIGRATION FOLDER IN THE DATA.ACCESS FOLDER

 2:20
 I tried to install the Nuget Package but it was unsuccessful, issue with my namespace

 2:56
 mY ERRORS KEEPS INCRESING BUT I REALISED I DIDNT DOWNLOAD THE MICROSOFT.ASP.NERCORE
 
 5:36
 All errors gone

 5:37
 i changed my namespace in my ApplicationDB.Context to  RobiatsBookStore.DataAccess.Data
5:38 
Moved the models folder into my books.Models and deleted the original one
I added the project reference in my dataAccess folder ,also renamed the models folder to ViewModels

5:40
i changed the ErrorViewModels.cs namespace to the Models.ViewModels and built the project it is working 
in my startup.cs file i have the ApplicationDbContext highlighted in red i clicked on it and it brought out suggestions adding the  .DataAccess.Data as my namespace

5:50
i had errors so i had to remove the RobiatsBookStore .Data i reviewed the browser presentation and everything was working perfectly

5:52
In the Utility project,i crweated a static detailed calss called SD.cs and modified the properties adding the public static i also added project reference in the 
main project sellecting all the three projects  RobiatsBooksStore.DataAccess,
 RobiatsBooksStore.Models,
 RobiatsBooksStore.Utility

 5:55
 in the dataAccess project i added the references to reflect Models and the utility
 i proceeded to add the customer area to the areas but received errors
i meen to make changes where i previously have my  ErrorViewModels to Models.ViewModels i got errors from my startup.cs and the ErrorViewModels i was supposed to 
do that earlier

6:36
it took me some moments to figure out where to change all the defaults but it is done now all errors gone and my customer area is added to my areas

6:37
i changed the routes in the startup.cs like the one outlined in my scaffolding readme adding  {area:exists}
i moved the HomecONTROLLER.CS TO THE ARE IN THE CUSTOMERS FOLDER AND I DELETED THE dATA AND mODELS FOLDERS

6:38
I EDITED THE homeController.cs to explicitly define the controller in the customer Area
6:40
I moved the view,home and i modified the HomeController namesace to add the RobiatBookStore.Controllers

6:42
i ran the application and the error i got is entirely different from what i am supposed to get
it says cant locate localhost

7:00
i figured it out,in my startup.cs i was supposed  to direct my area to the customer,instead of this {area:exists}
i was supposed to have this {area:Customer}

7:03
i moved my view import and the viewStart to the customer Area
i modified the viewStart.cshtml  to reflect the new path and i ran the application and it is working perfectly

7:10
in my area i added a new admin area and copied and pasted my viewimport.cshtml and the viewstart.cshtml 

7:15
i deleted the data and models folder and also deleted the controllers folder 
DONE!!!

2023-10-31 2:47
i started my part twofor the assignment 2
i cleaned and rebuilt my application and everything works perfectly

2:45
i went to my appsettings.json file and reviewed the code in it,i also changed the database name to Database=RobiatsBookStore and i saved it in my manager consOle

2:50
i added the migration using add-migration AddDefaultIdentityMigration but i got an error because my default project is the RobiatsBookStore instead of the DataAccess project folder
I RAN THE COMMAND AGAIN AND THE MIGRATION IS INSTALLED SUCCESSFULLY

2:59
the new migration added name is 20231031185239_AddDefaultIdentityMigration.cs
i went through the migration file and the tables created by the migration

3:06
i updated the database and it was successful

3:20
i created a category model in my model project and i modified it 

3:25
I added the migration in my PM Console to update my database   20231031192744_AddCategoryToDb.Designer STOP FOR NOW


2023-11-3 3:00

started by cleaning and buliding my project and also to run to see if everything is working perfectly

3:15 
i started by re-running the add-migration in my PM but i had errors and the building failed
could not access the category class

3:20
I went back to check what i did wrong in mycategory.cs file and realised i didnt ADD PUBLIC TO THE CLASS CATEGORY

3:30
 I DECIDE TO RUN THE add-migration again and i got the duplication error

 3:32
 I had to delete the migration previously added in my migration folder and run the command again


 3:35
 it is successful  the migration 20231103193916_AddCategoryToDb successfully added

 3:40
 i updated the database and my categories table has been added to the database'

 3:45
 i started the part 2.2 which is building the repository
 i added a new folder in my project.dataAccess which is the repository folder and in my repository folder
 i created another folder which is the IRepository folder
    
3:50 
in my IRepository folder i created an interface class named IRepository.cs and added the new item in my project.DataAccess.csproj file

3:55
I modified my IRepository.cs file so that i can perform the CRUD operations and also made changes in the using statement

4:00
IN MY REPOSITORY FOLDER I CREATED A rEPOSITORY.CS class 
i implemented the using statement and used the implement interface to fix my issues

4:15
I modified the code provided to me to create the constructors and dependency injection i was having little error so i used the suggested solutions and 
it fixed it through the using statements 

4:30
I used the file provided in the assignment 2 folder to modify the repository.cs file to create the constructors and dependency
injection DI

4:32
I CREATED INDIVIDUAL REPOS FOR CATEGORY AND THE POTENTIAL MODELS TO BE ADDED 

4:35
I created the CategoryRepository.cs and the IRepository.cs

4:50
I modified the CategoryRepository changed the using statements to specify my project

4:53
I also modified the ICategoryRepository interface 

5:00
i completeed the remaining modifications,built the project and everything is working perfectly

2023-11-6 12:00
I started by cleaning and building my project and everything works perfectly.i started by creating the interface class in my repository folder
called ISP_Call.cs which extends the IDisposable i included the methods shown and installed the NuGet package for the Dapper

12:10
i added a new class called the SP_Call.cs in the repository folder and selected the appropriate using statement and implemented the ISP_Call interface
after that i added a connection to the database and also updated the implemetation of the ISP_Call interface

12:40
i added the wrapper for the unit of work I CREATED A CLASS IN MY REPOSITORY CALLED unitsOfWorks and also created an interface in my IRepository called IUnitsOfWork
iupdated the code and modified the code to make sure the public class implements the interface UnitOfWork : IUnitOfWork

3:00
to mAKE IT ACCESSIBLE I WENT TO THE sTARTUP.CS in the ConfigureServices method  and added this  services.AddScoped<IUnitOfWork, UnitOfWork>();

3:15
I had errors when i added this code .AddScoped<IUnitOfWork, UnitOfWork>(); in my startup.cs file and i figured out i didnt add public at the 
beginning of the interface in my IUnitOf Work.cs everything is working perfectly now

3:30
in my controllers folder i added annew controller class called the categoryController.cs,i modified the code using the IUnitOfWork form the DataAccess project and
the IRepository folder adding the using RobiatsBooks.DataAccess.Repository.IRepository;

4:00
I added a new folder under my Areas/Views called Category and inside the category folder i created a new Index Razor view
and i used the code provided to edit the index.cshtml page for the layout

4:10
I edited the_layout.cshtml page to display my category button on the index page  i then moved the category link to the content management drop down
I reviewed the code and everything is working perfectly






2023-11-15 5:00

Started Part three of the project
I cleaned and built the project and everything was working perfectly
i started by adding the migration ADD cover type to the db 20231116024753_AddCoverTypeToDb

2023-11-20 11:27
I created the CoverType following the same methods used for the Category CRUD in section two
I added the CoverType.cs in the Model's folder which includes the ID and the name

11:35
i added the CoverType to the Repository and also added the ICoverTypeRepository class in the Data Access project
also added the ICoverRepository interface in the IRepository folder

11:50
i added thE CoverType to the UnitOfWork and the IUnit of work

12:01
I added the CoverType to the NavBar on the home page 
i also added the CoverType Controller with the all required action methods
I created the CoverType Index View to use the data tables
i had a little issue with the script file linkage , i had three @ in the script linking part and i could proceed

12:15
issues fixed and everything is working perfectly
i added the upsert view to take care of creating and updating CoverType
and the delete CoverType is done using the API Call.
Tried and everything is working perfectly well

12:20
Started with creating the Product CRUD
i created a product class in the models and added the product to the database
i added the migration  20231120174109_addProductToDb


2:00
I created  the product class to the model project and added the the migration
i got an empty migration
the product was not added to the database i dont know what i did wrong

2:30
still trying to figure out what the error is 
figured it out i was supposed to add the  public DbSet<Product> Products { get; set; } after the migration
i did it again and it is working perfectly i updated the database


3:00
i updated the product class so that the title isbn and the author are not left empty,i added the migration to the database
i updated the database and everything is working perfectly fine
i added the product to the repository and added the IProductRepository interface also made some changes in the update method in the ProductRepository 
i added the product of unit of work and ther Iunit of work
built the project and everything is working perfectly

6:00
I created a product Controller in the Areas,Admin Controller to perform the CRUD operation
I added the IWebHostEnvironmrnt and i added it using statement to the INCLUDE THE using Microsoft.AspNetCore.Hosting;
using Microsoft.AspNetCore.Mvc;

6:15
In the models project i created the ProjectVM class to hold the product object and select list for Category and the CoverType
I also modify the ProductVM class so that it is public and i installed the Microsoft.Asp.NetCore.Mvc.ViewFeaturespackage
Imodified the ProductController so the IActionResult Upsert to call the ProductVM view mode
i included the using RobiatsBook.Models.ViewsModels;
using Microsoft.AspNetCore.Mvc.Rendering; and all errors gone

6:20
I modified the API call to include th category and the CoverType properties
i added an index view and copied the code from my index.cshtml from the Views/category and used it to modify my product
and modified my code to include the Title,ISBN,Price,Author and the category  and i also created a product.js file
i linked m project with the product.js file i created earlier

7:00
I created an Upsert.cs for products and modify in Area/Admin/Views and i used the product file provided for us in the assignment folder 
i also added a rich textbox to the text are inside the product with the tiny.cloud by creating an account and using the api key generated
i checked the product create button and everything is working perfectly

2023-11-21 2:43
I created a new folder and subfolder in the wwwroot/images/products
in the productController i configured the product Upsert Post action method
i checked the project and it is working perfectly
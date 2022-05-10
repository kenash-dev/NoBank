If you have new update in database and want to update dbcontext, just add -f at end. It will update and overwrite all your dbcontext and model classes.
Scaffold-DbContext "Server=yourserveraddress;Database=yourdatabase;user id=youruser;password=yourpassword;" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models -Context "YourOwnContext" -f

If you want to add some data annotations such as [Column], etc in model class, can add -DataAnnotations
Scaffold-DbContext "Server=yourserveraddress;Database=yourdatabase;user id=youruser;password=yourpassword;" Microsoft.EntityFrameworkCore.SqlServer -OutputDir Models -Context "YourOwnContext" -DataAnnotations -f
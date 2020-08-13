# Policies 

To add a policy to an app, apply the following code snippet with the appropriate information. 

```csharp
  services.AddAuthorization(options =>
  {
      options.AddPolicy("Admin", policy => policy.RequireRole(AppRoles.Admin));
      options.AddPolicy("Users", policy => policy.RequireRole(AppRoles.Admin, AppRoles.User));
  });
  ```

  Then, apply this policy to the desired controllers OR Razor page.

  ```csharp
[Authorize(Policy = "Admin")]
public class AdminDashboard : Controller
{
    public IActionResult Index() => View();
}
  ```

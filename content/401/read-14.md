# Routing

### Routing With MVC

The ASP.NET routing module handles all incoming browsers requests and connects them to the appropriate controller actions.

When starting an MVC application, a few things happen:

1. The Application_Start() method is called
2. The above method then calls the RegisterRoutes() method.
3. The RegisterRoutes() method then creates the route table.

The route table comes configured with a default route. This route contains:
- The controller name
- The controller action
- The parameter 

Example:
Route: /Home/Hotel/4

Home -> controller name
Hotel -> controller action
4 -> parameter

---

### Routing in ASP.NET Core 

*What is routing?*

Routing connects inbound HTTP requests to the application endpoints.

*What is an endpoint?*

Endpoints are request-handling methods within the application.

Routing uses middleware that is configured with following methods:

```csharp
App.UseRouting();
App.UseEndpoints(...){...};
```


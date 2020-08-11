# Razor Pages

### What is it?

**Razor Pages** focuses on making cshtml pages that are heavy on coding much easier to use.

Be sure to enable razor pages in the *startup.cs* file.

```csharp
    public void ConfigureServices(IServiceCollection services)
    {
        services.AddMvc();
    }

    public void Configure(IApplicationBuilder app)
    {
        app.UseMvc();
    }
```

Within the razor page, use *@page* at the very top. This tells the compiler that it is a razor page and not an MVC view.

The architecture of razor pages is different than that of MVC. There is no 'Views' or 'Controllers' folders. The razor pages are inside of a folder named 'Pages'.

Razor pages is more lightweight than MVC.

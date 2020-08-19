# OAUTH

### What is it?

OAUTH is a way of signing in using external credentials. We do this all the time using google, microsoft or github accounts. 

---

### How to implement OATH

In the startup file, add the following desired lines of code:

```csharp
services.AddAuthentication()
  .AddMicrosoftAccount(microsoftOption => { ... })
  .AddGoogle(googleOptions => { ... })
  .AddTwitter(twitterOptions => { ... })
  .AddFaceBook(facebookOptions => { ... })
```

This code snippet was used from the [Microsoft Documentation](https://docs.microsoft.com/en-us/aspnet/core/security/authentication/social/?view=aspnetcore-2.1&tabs=visual-studio)




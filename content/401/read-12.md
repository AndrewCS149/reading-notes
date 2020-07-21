# EF Core & API's


---

### EF Core

EF (entity framework) Core is a cross-platform framework allows developers to work with a Database without having to use the traditional data-access code. Instead, .NET objects can be used.

**Importing EF Core**

```csharp
using Microsoft.EntityFrameworkCore;
```

In conjunction with LINQ, data can be accessed as follows:

```csharp
using(var db = new Locations()) 
{
  var pop = Locations.Population
      .where pop > 50000
      .OrderBy Descending
      .ToList();
}
```

---

### Data Seeding

Data seeding means to creating a database with already pre existing data.

There are three ways to achieve this:

1. Model Seed Data
2. Manual Migration Customization
3. Custom initialization logic

---

### User Secrets


*What is a user secret?*

A **user secret** is a method in which to store information private to a user (API keys). Anything that a user does not want others to know is a user secret.

**Viewing User Secrets**

1. Right click on project
2. Choose "Manage User Secrets"

Json file will open with: 

```json
{
  "myBingAPIKey": "{VALUE}",
  "textAPIKey": "{VALUE}",
  "ConnectionStrings": {
    "AzureConnection": "{CONNECTION STRING HERE}"
}
```






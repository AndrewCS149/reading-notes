# Classes & Memory Management
---

---
## Classes 

A class if a reference type, which means that it needs to be *explicity* created by using the **new** keyword.
---
```csharp
MyClass test = new MyClass();
```
---
**Class Declaration:**
```csharp
public class Dog
{
  // Fields
  // Properties
  // Methods
}
```
The **public** keyword is the access level of the class. This means that other classes can access this classes methods and properties.
---
Creating an instance of a class
```csharp
MyClass test = new MyClass();
```
---
**Class Inheritance**
This means that a class can *inherit* other classes methods and properties or override other classes methods. To extend (inherit) from another class:
```csharp
public class Dog : Animal
{
  // Fields
  // Properties
  // Methods
}
```

---
## Constructors

A class instance is created with a **constructor**. Constructors are used to give the instance default values. It is possible for a class to have more than one constructor. 
---
**Constructor Syntax**
```csharp
public class Dog 
{
  private string breed;
  private string gender;

  public Dog(string breed, string gender)
  {
    this.breed = breed;
    this.gender = gender;
  }

  // methods
}
```

---
## Properties

A **property** is a member of a class that allows easy data manipulation to specific areas of that class. This data is very easy to access.

---
## Stack & Heap

The **stack** keeps track of whats actually being executed in the code base, while the **heap** keeps track of objects.
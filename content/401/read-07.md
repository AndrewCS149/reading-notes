# OOP Principles
---

| O      | O        | P           |
| ------ | -------- | ----------- |
| OBJECT | ORIENTED | PROGRAMMING |

Three pillars of object oriented programming:

* **Encapsulation**
* **Inheritance**
* **Polymorphism**

---

## Inheritance

**Inheritance** allows for class characteristics, such as methods and properties, to extend to other classes for reuse amongst similar objects.

**Base Class** - The class from which other classes are *inheriting* from (also known as *hero*).

**Derived Class** - The class the is *inheriting* the base class characteristics.

**Example:**

```csharp
// BASE CLASS
class Animal
{
  public string name;
  public int age;
  public int weight;

  public void PrintBase ()
  {
    Console.WriteLine($"Name: {name}.");
    Console.WriteLine($"Age: {age}.");
    Console.WriteLine($"Weight: {weight}.");
  }
}

// DERIVED CLASS
class Dog : Animal
{
  public string breed; 

  public void Bark() 
  {
    Console.WriteLine("WOOF!");
  }
}

// DERIVED CLASS
class Cat : Animal
{
  public float cuteness;

  public void Meow() 
  {
    Console.WriteLine("meow");
  }
}
```

*example influenced by 'Brackeys'* [youtube video](https://www.youtube.com/watch?v=EiBCF7rYRtI)

---

## Abstraction

If a user wants to create class without having to instantiate that class, then an **abstract class** should be used.

Abstract class declaration:

```csharp
public abstract Class A
{
  /// class stuff
}
```

---

## Polymorphism

**Polymorphism** allows *derived classes* to override methods inherited from the *base class* and change them as needed.

Example:

```csharp
class Person
{
  public virtual void SayHi()
  {
    Console.WriteLine("Hello! I am a person.");
  }
}

class Andrew
{
  public override void SayHi()
  {
    Console.WriteLine("Hello! My name is Andrew.");
  }
}
```

**Virtual method** allows *derived classes* to choose whether to override those methods or not. If the virtual keyword is omitted, the derived class cannot override the 'SayHi()' method from the base class.

The **override** keyword must also be part of the method signature within the derived class. If this omitted, it will inherit the same method from the base class.

---

## Structures 

**Structures** are used when inheritance and polymorphism is not needed.

Defining a class as a structure:

```csharp
struct ClassA
{
  // class info
}
```

The difference between a **class** and a **struct** is that a class is a reference type, while struct is a value type.

*But what is the difference between a reference type and a value type?*
 * Reference types are contained within the heap, while values are contained within the stack.
 * Reference type arrays are distributed *out-of-line*, meaning that the array is only referencing instances inside of the heap. Value type arrays are distributed *inline*, meaning that they are not referencing instances, but they are the actual instances.

---

## Class Members - properties | fields | methods

**Class Members** are the properties, fields and methods that make up the class. 

#### Fields & Properties

Defining fields & properties:

```csharp
class ClassA
{
  // field
  string name;

  // property
  public int Age { get; set; }
}
```

As seen above, the properties have the **set** & **get** **accessors**. This gives more control on how these values are accessed or changed.





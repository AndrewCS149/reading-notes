# Collections & Enums
---

## Collections

A **collection** is a way to group similar objects. An array is another way to do this. 

*What is the difference between collections and arrays?*

Arrays are useful for dealing with a fixed number of objects, while collections allow for an abstract number of objects. This means that a collection has the ability to add objects and remove them.

#### Instantiating a Collection

Because a collection is a class, an instance must be created before the collection can be used. 

#### Different Collections

If only one data type is desired, then it is safe to use a collection from the 'generic' namespace. The generic namespace can be imported as:

`using System.Collections.Generic;` 

AND

`using System.Linq;`

When using a generic collection, various data types are not allowed.

Generic collection example:

```csharp
// declare new list and add to it
string people = new List<string>();
people.Add("Andrew");
people.Add("Courtney");
people.Add("Dale");

// print out all items
foreach (string name in people)
{
  Console.WriteLine(name);
}
```

The elements can also be added to the list at the same time of the instantiation:

```csharp
string people = new List<string> {"Andrew", "Courtney", "Dale"};
```

Removing elements from a list:

```csharp
people.Remove("Andrew");S
```

Different Collections.Generic types:

| Class                    | Description                            |
| ------------------------ | -------------------------------------- |
| List<T>                  | List of objects with idx's.            |
| Dictionary<TKey, TValue> | Collection of key/value pairs          |
| Queue<T>                 | FIFO (First in, first out)             |
| SortedList<TKey, TValue> | Key/value pairs that are sorted by key |
| Stack<T>                 | LIFO (Last in, first out)              |

#### Dictionaries

Dictionaries use **key/value** pairs.

Initializing a dictionary:

```csharp
Dictionary<string, int> people = new Dictionary();
```

Adding to a dictionary:

```csharp
people.Add("Andrew", 25);
people.Add("Courtney", 23);
people.Add("James", 27);
```

---

## Enumeration Types (Enums)

An **enum type** is a **value type** representing **constants**. A constant is a read-only variable that cannot be manipulated.

Declaring an enum:

```csharp
enum Directions
{
  North,
  East,
  South,
  West
}
```

By default, the values of enum members will be of type int and start at zero. Different int values can be explicitly declared like so:

```csharp
enum People 
{
  Andrew = 25,
  Courtney = 23,
  James = 27
}
```


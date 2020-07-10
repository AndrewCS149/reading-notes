# Linked Lists
---

A **linked list** is a bunch of nodes that are connected to each other. Each node references the very next node.


### Terminology

* **linked list** - Data structure of nodes that references the next node in the list
* **singly** - There is only *one* reference that points to the *next* node in the list
* **doubly** - There are *two* references that point to the *next* and *previous* node in the list.
* **node** - Individual list items.
* **next** - Property that references the *next* node.
* **head** - Reference type of the first node in the list.
* **current** - The current reference type of the current node.

A for loop and foreach are both incompatible with a linked list. The next keyword is what iterates through the list.

### Declaring a linked list

```csharp
string[] cars = {"bmw", "ram", "tesla", "ford", "honda"};
LinkedList<string> linkedCars = new LinkedList<string>(cars);

// print out all nodes

string current = Head;
while(current.Next != Null)
{
  Console.WriteLine(current);
  current = current.next;
}
Console.WriteLine(current);
```


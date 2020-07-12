# LINQ
---

| L        | IN         | Q     |
| -------- | ---------- | ----- |
| Language | Integrated | Query |

LINQ is exactly what the name implies, an integration of query functionality. The LINQ collection is the same queries as one might find in a relational data base management system such as SQL. LINQ is a simplistic way to push data into a database or extract information from enumerable objects in a query syntax.

---

### Using a LINQ query

To use the query capabilities of LINQ, an IEnumberable collection must be created. This is contained in the Collections.Generic namespace.

```csharp
int[] numbers = new int[] { 10, 20, 30, 40 };

IEnumerable<int> numbersQuery =
    from number in numbers
    where number > 20
    select number;

foreach (int num in numbersQuery) 
{
  Console.WriteLine(num);
}
```

---

### Using LINQ with a database

To query database information, a database must be set up and a `IQueryable<T>` must be used to query the data.

```csharp
// Set up database
StoreLocations db = new StoreLocations(@"C:\path\to\db")'

// Query all customers at the Seattle location
IQueryable<Customer> custQuery = 
    from cust in db.Seattle
    select cust;
```
---
### Joining

**Joins** are used to link two database tables in a singe query, thus retrieving data from two tables simultaneously. 

```csharp
var customersEmployeesJoin = 
    from cust in customers
    join employees using name;
```


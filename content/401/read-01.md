# Exception Handling

---

## Debugging for Beginners 

It is important to ask yourself questions about what went wrong. Start with these basic questions: 

* What did you want your code to do?
* What did your code actually do?

Use the debugger tool to incrementally step through the script to pin point the actual location of the bug. 

The debugging process can begin with the **green play button** or the **F5** key. 

---

## Try / Catch 

If a potential error is expected, place that code inside of a `try` block. Then place the code that will **handle** that error inside of a `catch` block.

```csharp
try
{
  nums[i] = 10;
} catch(IndexOutOfRangeException) 
{
  Console.WriteLine("Sorry, that item does not exist.");
}
```

---

## Statement Keywords

Here is a list of c sharp statement keywords.

| Category                      | C# Keywords                                      |
| ----------------------------- | ------------------------------------------------ |
| selection statements          | if, else, switch, case                           |
| iteration statements          | do, for, foreach, in, while                      |
| jump statements               | break, continue, default, goto, return, yield    |
| exception handling statements | throw, try-catch, try-finally, try-catch-finally |
| checked & unchecked           | checked, unchecked                               |
| fixed statement               | fixed                                            |
| lock statement                | lock                                             |


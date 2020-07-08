# Systems.IO
---

---
## File and Stream I/O 
---

File and stream input / output is actually referencing the process of data transfers from or to a storage location. 


---
## Writing to a file
---

Methods and classes used to write to a file:
* StreamWriter
* File
* path


StreamWriter methods writes to files synchronously.

File methods write text to a file. Example:
* WriteAllLines
* WriteAllText
* AppendAllLines
* AppendAllText

---
## Reading from a file
---

The classes 'System.IO.BinaryWriter' & 'System.IO.BinaryReader' are used to read and write non strings characters to files. 
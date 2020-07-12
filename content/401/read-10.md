# Stacks & Queues
---

## Stacks

*What is a stack?*

Stacks are data structures that contain nodes and each node references the next sequential node in the stack.

Stacks terminology:

* **Push** - Adding nodes to the stack
* **Pop** - Nodes that are removed from the stack
* **Top** - Top of the stack
* **Peek** - Viewing the top node
* **IsEmpty** - If the stack is empty, return true, otherwise, return false

#### FILO

| F     | I   | L    | O   |
| ----- | --- | ---- | --- |
| First | In  | Last | Out |

#### LIFO

| L    | I   | F     | O   |
| ---- | --- | ----- | --- |
| Last | In  | First | Out |

#### Big O

* Push - O(1)
* Pop - O(1)
* Peek - O(1)
* IsEmpty - O(1)

---

## Queue

Queue Terminology:
* **Enqueue** - Nodes added to queue
* **Dequeue** - Nodes removed from queue
* **Front** - First node of queue
* **Rear** - Last node of queue
* **Peek** - View front node of queue
* **IsEmpty** - Return true of queue is empty, false if not

#### FIFO

| F     | I   | F     | O   |
| ----- | --- | ----- | --- |
| First | In  | First | Out |

#### LILO

| L    | I   | L    | O   |
| ---- | --- | ---- | --- |
| Last | In  | Last | Out |

#### Big O

**Enqueue**, **Dequeue**, **Peek** and **IsEmpty** are all O(1) operations.


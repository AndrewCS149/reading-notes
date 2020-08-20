# Red-Black Trees

### What is it?

A *Red-black tree* is similar to a binary search tree, but each node has a color attribute to it as well. Here are some properties that exclusive to red black trees:

- Root is black
- Leaves are black
- Red nodes can only have black child nodes
- Nodes to leaves contain the same number of black nodes

This help keeps the tree ordered and as wide as possible, which increases the lookup times.

---

### Code

```csharp
RedBlack rb = new RedBlack();

// Methods
rb.GetMinKey();
rb.GetMaxKey();
rb.GetMinValue();
rb.GetMaxValue();
rb.GetEnumerator();
rb.Key();
rb.Values();
rb.RemoveMin();
rb.RemoveMax();
```
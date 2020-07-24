# Trees

### Common Terms

- *Node* - Each single node
- *Root* - The node at the top of the tree
- *Left* Child - Node that is left of the root or node
- *Right* child - Node that is right of the root or node
- *Edge* - The connection from a child node to a parent node
- *Leaf* - A node that has no children
- *Height* - Number of edges from the root to the bottom node
 
---

### Travesering a Tree

There are two ways to traverse a tree:

- **Depth First**
- **Breadth First**

*Depth First* means to traverse it's height.

*Breadth First* traverses each level on the tree.

---

### Binary Trees

Binary search trees can only have TWO children per node. 

When adding a node, it doesn't matter where it is placed, as long as it it placed at the bottom. The time complexity for adding a node is O(n).

---

### Binary Search Trees

Unlike binary trees, there is some order to a binary search trees. All nodes that have values greater than the root node are placed on the left, while all nodes with values greater than the root node are placed on the right. 

Big O time complexity for inserting or searching in a binary search tree is O(h), where h represents the height of a tree. We will only have to search all the way down to a single leaf in worst case scenario. 

Big O space complexity for a binary search tree search is O(1) because no additional memory is being allocated. 

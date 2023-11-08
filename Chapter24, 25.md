## Trees



* Can be an ADT and a Data  Structure

![Tree Visual](https://raw.githubusercontent.com/RamziCarter/DataStructures1/main/TreesEx.png)


Definitions
---

```
Parent - 
Children - 
Assestor - 
Descendent - 
Leaf - 
Path - 
```

---

Binary Tree - every node has no more than two children 
> Able to have 0, 1 or 2 children

Subtree - Pick a node, everything underneath it is a subtree

**Length of a path** - number of edges in a path


**Height of the tree** - number of nodes in the longest path


#### Checking the entire tree
> Part 1
* visit every node in the tree

> Part 2




---
## Tree Traversals

* Inorder -  the node itself is between the two children (Left child, Node, Right Child)
* PreOrder - visit thew node itself then visit the left child then right child
* PostOrder - Left Child, Right Child, Node
* DepthFirst
* BreadthFirst - Visit each level from left to right over the entire tree
* 

---



```java
// Tree Interface
// what is missing from the interface?



```

> Binary Search Tree

* for a binary tree to be searchable the data in every left descendant of the node must be less than the data in the node 

**Complete and Full Trees**
A Full Tree

* a tree is a binary tree where there are 2^(n-1) nodes
* every node has two children or no children making it a leaf
   * searching a full tree is the most efficient with an average of O(log N)

A Complete Tree

* 

# Trees
### Trees consists of nodes which are connected with each other.
### Common Terminology for Trees:
- Node is a Tree node is a Tree component, has it’s own values, and references to other nodes
- `Root` is the node at the beginning of the tree
- `K` is a number specifies the maximum number of children any node can have
- `Left` is a reference to one child node, in a binary tree
- `Right` is a reference to the other child node, in a binary tree
- `Edge` is the edge in a tree is the link between a parent and child node
- `Leaf` is a node that does not have any children
- `Height` of a tree is the number of edges from the root to the furthest leaf
### Trees are divided into three parts which are:
- Binary Trees
- Binary Search Trees
- K-ary Trees
### Traversals is how to search for a node in a Tree. There are two categories of traversals for trees:
- Depth First
    - traversal in depth first is where we prioritize going through the depth (height) of the tree first
- Breadth First 
    - traversal in breadth first iterates through the tree by going through each level of the tree node-by-node
## K-ary Trees
### K-ary Trees exists when Nodes are able have more than two child nodes
### Big O for time complexity for inserting a new node is O(n). Searching for a specific node will also be O(n). 
### The Big O for space complexity for a node insertion using breadth first insertion will be O(w), where w is the largest width of the tree. For example, in the above tree, w is four
## Binary Search Trees
### Binary Search Trees is exists when nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.
### Big O for time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height) and in the worst case it will be log(n)
### The Big O space complexity of a Binary Search Tree search would be O(1)

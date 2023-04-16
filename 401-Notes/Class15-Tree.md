# Trees

## What is a tree?

A tree is a data structure consisting of a set of linked nodes that represent a hierarchical tree structure. Each node is linked to others via parent-children relationship. The first node in the tree is the root, whereas nodes without any children are the leaves.

## Terminology

1. Node - A Tree node is a component which may contain its own values, and references to other nodes
2. Root - The root is the node at the beginning of the tree
3. K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
4. Left - A reference to one child node, in a binary tree
5. Right - A reference to the other child node, in a binary tree
6. Edge - The edge in a tree is the link between a parent and child node
7. Leaf - A leaf is a node that does not have any children
8. Height - The height of a tree is the number of edges from the root to the furthest leaf

## Tree Visualization

![Tree](401-Notes/assets/Tree.png)

## Traversals

An important aspect of trees is how to traverse them. Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees:

- Depth First
- Breadth First

### Depth First

Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root. Here are three methods for depth first traversal:

Pre-order: root >> left >> right
In-order: left >> root >> right
Post-order: left >> right >> root

### Breadth First

Breadth-first traversal means that we start from the top node, then go one level down, go through all of the children nodes from left to right.


[link-to-reading-notes](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?
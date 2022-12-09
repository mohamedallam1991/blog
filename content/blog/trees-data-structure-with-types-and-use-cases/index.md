---
title: "Trees data structure with types (uses cases included)"
slug: "trees-data-structure-with-types-and-use-cases"
date: 2022-12-09
description: "Trees are one of the prominent data structure out there, lets learn them step by step."
tags: ["golang", "dsa", "trees"]
showTableOfContents: true
thumb:
---

This articles breakdown the terminology used in trees data structure, as well as some types of trees and their use cases, to get familiar with them.

<!--more-->

# Trees types and use cases
## Whats a tree

A tree is a collection of nodes, each node holds some data, one of the nodes is the root node, and other nodes. are disjoints subsets and each subset is a tree or a sub tree.

Each node has exactly one parent, and can have one or more children, no single node has more than one parent.

Trees are everywhere:

- If you wrote any switch statement but didnt knew why its more efficient than a bunch of if-else statements, [the answer is Look up tables (LUT) which may use BST](https://en.wikipedia.org/wiki/Lookup_table)
- Operating systems use trees for [File system](https://en.wikipedia.org/wiki/File_system).
- The syntactic representation of a programming language is Abstract syntax tree. [AST](https://en.wikipedia.org/wiki/Abstract_syntax_tree)
- Browser Document object model ([DOM](https://en.wikipedia.org/wiki/Document_Object_Model))
- Databases use Log structured merge tree. [LSM](https://en.wikipedia.org/wiki/Log-structured_merge-tree) tree
- SQL index use [b-tree](https://en.wikipedia.org/wiki/B%2B_tree).
- Dynamic memory management uses [heap](https://en.wikipedia.org/wiki/Memory_management#Dynamic_memory_allocation). which is a type of a tree.
- A trie for dictionaries or [auto complete algorithms.](https://www.geeksforgeeks.org/auto-complete-feature-using-trie/)
- Priority queues as well use [heap](https://www.geeksforgeeks.org/priority-queue-using-binary-heap/).
- Garbage collectors also [use trees](https://en.wikipedia.org/wiki/Tracing_garbage_collection).

[https://en.wikipedia.org/wiki/Tree_(graph_theory)](https://en.wikipedia.org/wiki/Tree_(graph_theory))

[https://en.wikipedia.org/wiki/Tree_(data_structure)](https://en.wikipedia.org/wiki/Tree_(data_structure))

### Nodes or vertices

Nodes is every unit of data

### Edges or paths (links)

Its the connection between each two nodes, if we have N nodes we would have N-1 edges, because each node as parent, except the root node.

### Root

Is the upmost node, who has no parent, and have only children,  for the children nodes this is their most parent node, generally in the top of the tree.

### Parent-Children

A node is a parent to its very next descendants. the descendants are the children to whom its connected with one single edge.

### Siblings

Are the children connected to the same node.

### Descendants

When we want to talk about children and their children, and the children of their children..etc we would say descendants.

It means the set of nodes we can reach from a particular node going to its children. so all the subtree.

### Ansestors

From that node to the root node, all this nodes are considered anscestors.

### Degree of nodes

Is the number of children a node has, so the direct children.

A degree of a tree cannot be told from a tree, but its predefined, we can say its a binary tree. but if its unbalanced, we would see it in a form of a linkedlist.

### Leaf nodes, external or terminal

All nodes who has no children. so with nodes with degree 0

### Levels

Levels starting from first level 1, the root, as we categorize each level by all the nodes who take the same number of edges to get to the root node.

### Height

Hight of nodes, is the same as the levels but it starts from 0, its very useful for analysis.

### Forest

A collection of a tree is called a forest. which at least has a root node.

To convert a forest to a tree, we attach the roots of the present trees, to one single root.

## Types of trees

There is many types of trees, and they are extremely useful and popular. for example

### Binary tree

One of the most popular trees, is [the binary tree](https://en.wikipedia.org/wiki/Binary_tree),

Its tree of degree 2, means every node can have 0,1 or 2 children, but not more than 2.

$deg(T)=2$

$children={{0,1,2}}$

- Because the nodes can have only 2 nodes, we call them left child and right child. or left node and right node.
- If we come across a tree that is unbalanced, means it forms something like a linked list, but to the left side, we call it left skewed binary tree. or right skewed binary tree

### Binary search tree

The binary search tree or [BST](https://en.wikipedia.org/wiki/Binary_search_tree) , is a derivate of binary tree, but with a constraint in the data, Its a rooted binary tree, where every node (data) on the left side is grater than nodes on the right side.

$deg(T)=2$

### AVL Tree

Another tree named after inventors **A**delson-**V**elsky and **L**andis, is a self balancing binary search tree.

### Decision Tree

Its one of the popular ones for [classification and prediction](https://www.geeksforgeeks.org/decision-tree/).

### Fenwich Tree

A Fenwick tree or binary indexed tree is a data structure that can efficiently update elements and calculate [prefix sums](https://en.wikipedia.org/wiki/Prefix_sum) in a table of numbers.

Link to [wiki](https://en.wikipedia.org/wiki/Fenwick_tree)

### Log structured Merge Tree

Or LSM [tree](https://en.wikipedia.org/wiki/Log-structured_merge-tree)  one of the trees used in databases like influxDB.

# AVL Trees

This repository contains a **simple yet comprehensive implementation** of **Binary Search Trees (BSTs)** and **AVL Trees (self-balancing BSTs)** written from scratch in **C++**.

## Features
- **Binary Search Tree (BST)**: Standard implementation with insertion, deletion, and traversal.
- **AVL Tree**: Self-balancing BST ensuring O(log n) insertion and deletion.
- **Iterator Support**: Enables in-order traversal using iterators.

## Public Interface

```C++
void insert(std::pair<const Key, Value> new_item);
void remove(Key key);
```

### Example Usage

```C++
#include "AVLTree.h"

AVLTree<char, int> testTree;
testTree.insert(std::make_pair('a', 1));
testTree.insert(std::make_pair('b', 2));

for (AVLTree<char, int>::iterator it = testTree.begin(); it != testTree.end(); ++it) {
    std::cout << it->first << " " << it->second << std::endl;
    // Output:
    // a 1
    // b 2
}

testTree.remove('b');

return 0;
```

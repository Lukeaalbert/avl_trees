# avl-trees

This repo includes a simple but comprehensive implementation of the binary search tree and AVL tree (self-balancing BST) data structures written in C++.


The public interface for an AVL tree is:
```C++
    void insert (std::pair<const Key, Value> new_item);
    void remove(Key key);
```
and sample usage may look like:
```C++
AVLTree<char,int> testTree;
testTree.insert(std::make_pair('a',1));
testTree.insert(std::make_pair('b',2));

for(AVLTree<char,int>::iterator it = at.begin(); it != at.end(); ++it) {
  cout << it->first << " " << it->second << endl;
  // a 1
  // b 1
}
at.remove('b');

return 0;
```


AVL trees have O(logn) insert and delete operations, making them an awesome and wonderfully efficient data structure!

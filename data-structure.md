# Data structure

↑ **Parent:** [Computer science](computer-science-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Data_structure)

A [data structure](data-structure.md) organizes stored information together with operations for accessing and changing it. Choosing a [data structure](data-structure.md) means choosing which questions should be cheap to answer: an [array](array-data-structure.md) supports access by numbered position, a [hash table](hash-table.md) supports lookup by key, and a [priority queue](priority-queue.md) supports selecting an item by priority. The operations and their [time complexity](time-complexity.md) matter as much as the stored values.

Suppose three requests arrive as $(5,\mathrm{Ada}),(2,\mathrm{Bo}),(4,\mathrm{Cy})$, where the number is a priority and smaller numbers are more urgent. A [FIFO queue](fifo-queue.md) removes Ada first because she arrived first. A minimum-oriented [priority queue](priority-queue.md) removes Bo first because $2$ is the least priority. An [array](array-data-structure.md) can store the same three records in arrival order, but finding the least priority by scanning this representation takes three key inspections. A [binary heap](binary-heap.md) organizes these records so the least priority is immediately available. The information is the same; the representation changes the work needed to use it.

This is a useful design principle: preserve just enough organization for the operations the application needs. Maintaining a [sorted array](sorted-array.md) gives the whole order, but moving entries to insert a new key can be expensive. A [binary heap](binary-heap.md) keeps a weaker [heap order](heap-order.md) that supports fast repeated selection without maintaining a [sorted array](sorted-array.md). A good [data structure](data-structure.md) makes an [algorithm](algorithm.md)'s next step easy.

**Table of contents**

- [Adjacency list](adjacency-list.md)
- [Priority queue](priority-queue.md)
  - [Binary heap](binary-heap.md)
    - [Heap order](heap-order.md)
    - [Sift up](sift-up.md)
    - [Sift down](sift-down.md)
- [Hash table](hash-table.md)
  - [Separate chaining](separate-chaining.md)
    - [Simple uniform hashing](simple-uniform-hashing.md)
  - [Hash bucket](hash-bucket.md)
  - [Key equality](key-equality.md)
  - [Load factor of a hash table](load-factor-of-a-hash-table.md)
  - [Hash table resizing](hash-table-resizing.md)
- [Array (data structure)](array-data-structure.md)
  - [Row-major order](row-major-order.md)
  - [Column-major order](column-major-order.md)
  - [Sorted array](sorted-array.md)
- [Circular buffer](circular-buffer.md)
- [FIFO queue](fifo-queue.md)
  - [Two-list functional queue](two-list-functional-queue.md)
- [Stack (data structure)](stack-data-structure.md)
  - [Call stack](call-stack.md)
- [Binary tree](binary-tree.md)
  - [Subtree](subtree.md)
  - [Height of a binary tree](height-of-a-binary-tree.md)
  - [Inorder traversal](inorder-traversal.md)
  - [Binary search tree](binary-search-tree.md)
    - [Dictionary intersection](dictionary-intersection.md)
  - [Complete binary tree](complete-binary-tree.md)
  - [Full binary tree](full-binary-tree.md)
- [Linked list](linked-list.md)
  - [Linked list node](linked-list-node.md)
  - [Mutable list](mutable-list.md)
  - [Lazy list](lazy-list.md)

## ↑ Ancestors (2)

1. [Computer science](computer-science-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Array (data structure)](array-data-structure.md)
- [Binary search tree](binary-search-tree.md)
- [Binary tree](binary-tree.md)
- [Bounding volume hierarchy](bounding-volume-hierarchy.md)
- [Buffered device block](buffered-device-block.md)
- [Computer science](computer-science-split.md)
- [Data structure](data-structure.md)
- [Encapsulation (computer programming)](encapsulation-computer-programming.md)
- [FIFO queue](fifo-queue.md)
- [File-system allocation bitmap](file-system-allocation-bitmap.md)
- [Hash function](hash-function.md)
- [Inode](inode.md)
- [Linked list](linked-list.md)
- [Page table](page-table.md)
- [Priority queue](priority-queue.md)
- [Stack (data structure)](stack-data-structure.md)

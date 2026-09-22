# Linked-list minimum extraction

↑ **Parent:** [Singly linked list](singly-linked-list.md)

Scan a nonempty [linked list](linked-list.md) while remembering the predecessor of its least-valued node. A [sentinel node](sentinel-node.md) supplies a predecessor even when the minimum is the first data node. Once the scan ends, bypass the selected node and detach its outgoing link. Using strict comparison retains the first occurrence among tied minima. Repeated extraction and tail-appending gives stable [selection sort](selection-sort.md) without replacing the data nodes or collapsing equal values.

## ↑ Ancestors (5)

1. [Singly linked list](singly-linked-list.md)
2. [Linked list](linked-list.md)
3. [Data structure](data-structure-split.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2017/imperative-programming/3/c/solution.md)

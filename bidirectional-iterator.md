# Bidirectional iterator

↑ **Parent:** [Iterator](iterator.md)

An [iterator](iterator.md) with forward and backward cursor movement. With the cursor between elements, `next` crosses and returns the element to the right, and `prev` crosses and returns the element to the left. Memoizing a forward-only source's consumed prefix supports arbitrary backward travel over that prefix without replaying source effects. The required history storage grows with the farthest explored position, even if the current cursor later moves backward.

## ↑ Ancestors (4)

1. [Iterator](iterator.md)
2. [Data structure](data-structure-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/7/b/solution.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2015/imperative-programming/7/c/solution.md)

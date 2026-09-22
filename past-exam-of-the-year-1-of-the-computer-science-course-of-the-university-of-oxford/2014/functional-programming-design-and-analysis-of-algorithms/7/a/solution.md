<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [maximum priority queue](../../../../../maximum-priority-queue.md) is an [abstract data type](../../../../../abstract-data-type.md) holding items with comparable priority keys and giving access to a greatest-key item. Equal priorities may occur; any one of the tied maximum items can be returned unless a tie rule is specified.

- `empty` or initialization creates a queue with no items; `isEmpty` and `size` inspect its occupancy.
- `insert(item, key)` adds an item with its priority.
- `maximum()` returns a greatest-priority item without removing it.
- `extractMax()` returns and removes a greatest-priority item.
- When mutable priorities are supported, `increaseKey(handle, newKey)` raises an existing item's priority; the handle identifies its stored location.

The central behavior is $\boxed{\operatorname{maximum}(Q)\in\operatorname*{arg\,max}_{x\in Q}\operatorname{key}(x)}$. Calling `maximum` or `extractMax` on an empty queue must report that no item exists. Raising a key is a common supported extension; arbitrary-key changes and deletion by handle can also be supplied.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

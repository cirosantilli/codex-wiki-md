<h1 id="5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The relevant quantity is the hash-table load factor $\alpha=n/M$, where $n$ is the number of distinct keys and $M$ the bucket count. With a suitable distribution of hashes, [separate chaining](../../../../../separate-chaining.md) has expected operation cost $O(1+\alpha)$, treating key operations as constant-cost. Keeping only one hundred buckets while $n$ grows therefore increases average search length.

Balanced [binary search trees](../../../../../binary-search-tree.md) could reduce a bucket search from linear time in its occupancy to logarithmic time. **Unbalanced [binary search trees](../../../../../binary-search-tree.md) provide no such guarantee**: insertion order can produce a chain. Even balanced trees add comparison and node-management overhead, which may dominate for small buckets.

A usual first remedy is **grow the table and rehash its entries, keeping the load factor bounded**. Geometric growth gives amortized constant resizing overhead per insertion; with suitable hashing, expected lookup, update and insertion costs remain constant. Resizing is $O(n)$ when performed and is not a worst-case constant-time guarantee for that particular operation. Balanced buckets can still be useful for heavy or adversarial collisions, but replacing every bucket tree does not by itself repair a poor [hash function](../../../../../hash-function.md). For variable-length [strings](../../../../../string.md), hashing and [string](../../../../../string.md) comparisons add their own character-processing costs.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

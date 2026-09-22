<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With a **directly indexed [array](../../../../../array-data-structure.md)**, use two parallel count [arrays](../../../../../array-data-structure.md), or one [array](../../../../../array-data-structure.md) of count records, at each user identity. Both queries and increments take $O(1)$ [running time](../../../../../running-time.md), with no [hash collision](../../../../../hash-collision.md). However, reserving $10^8$ positions for each of two four-byte counters uses about $800$ million bytes, roughly $763$ MiB before object overhead, even when only a few users have payments. Index zero is unused and all valid positions initially contain zero.

With a **[linked list](../../../../../linked-list.md)**, store one node `(user, countIn, countOut, next)` for each active user. A scan locates a record, returning zero counts if absent; an increment creates a missing record or updates its counter. Storage is $O(K)$ for $K$ stored users, but a query or update can require $O(K)$ [running time](../../../../../running-time.md). Nodes also carry pointer and allocation overhead and lack direct indexed access.

With a **[hash table](../../../../../hash-table.md) using [separate chaining](../../../../../separate-chaining.md)**, compute a [hash bucket](../../../../../hash-bucket.md) from the user identity and store its record in that bucket's [linked list](../../../../../linked-list.md). The same zero-default convention applies to a missing record. With $B$ buckets and a well-distributing [hash function](../../../../../hash-function.md), the expected operation cost is $O(1+K/B)$ in terms of the [load factor of a hash table](../../../../../load-factor-of-a-hash-table.md); worst-case cost remains $O(K)$ under severe collisions. Storage is $O(B+K)$, but a permanently fixed $B=100$ cannot maintain constant expected cost as $K$ grows without bound. A good distribution and, where permitted, [hash table resizing](../../../../../hash-table-resizing.md) address that trade-off.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

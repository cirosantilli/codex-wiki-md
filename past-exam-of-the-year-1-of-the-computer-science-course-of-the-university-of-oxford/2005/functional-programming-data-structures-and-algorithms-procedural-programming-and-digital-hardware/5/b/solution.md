<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Heapsort](../../../../../heapsort.md) uses $\Theta(n)$ time for [bottom-up heap construction](../../../../../bottom-up-heap-construction.md) and $O(\log n)$ for each extraction, giving $\Theta(n\log n)$ worst-case [time complexity](../../../../../time-complexity.md). An iterative [heapify down](../../../../../sift-down.md) on an [array](../../../../../array-data-structure.md) uses $O(1)$ auxiliary [space complexity](../../../../../space-complexity.md). Ordinary [heapsort](../../../../../heapsort.md) is not a [stable sorting](../../../../../stable-sorting.md) method.

[Quicksort](../../../../../quicksort.md) has balanced-case and average-case $\Theta(n\log n)$ [time complexity](../../../../../time-complexity.md) when the input order supplies suitably distributed pivot ranks. With the prescribed first-element pivot, sorted inputs produce subproblems of sizes $0$ and $n-1$, giving $T(n)=T(n-1)+\Theta(n)=\Theta(n^2)$. With the stated two-way partition convention, all-equal keys also give this worst case. There is no input-independent expected bound without a distribution or randomization assumption. For an in-place [array](../../../../../array-data-structure.md) implementation, the recursion stack is $O(\log n)$ when balanced and $O(n)$ in the worst case; the functional [list](../../../../../list-abstract-data-type.md) trace also allocates new partition spines and copied concatenation prefixes. Ordinary in-place [quicksort](../../../../../quicksort.md) is not [stable sorting](../../../../../stable-sorting.md); the stable-partition [list](../../../../../list-abstract-data-type.md) convention used in the trace can preserve equal-key order at additional allocation cost.

[Counting sort](../../../../../counting-sort.md) uses $\Theta(n+k)$ [time complexity](../../../../../time-complexity.md) for $k$ possible consecutive [integer](../../../../../integer-split.md) keys. The [stable sorting](../../../../../stable-sorting.md) version uses $\Theta(n+k)$ auxiliary [space complexity](../../../../../space-complexity.md) including the output [array](../../../../../array-data-structure.md); counting and re-emitting bare keys needs only $O(k)$ beyond its output. It is attractive when $k$ is small, but a sparse huge key range makes both initialization and count storage expensive. It relies on indexing by bounded [integer](../../../../../integer-split.md) keys, so it is not subject to the [comparison sorting lower bound](../../../../../comparison-sorting-lower-bound.md).

$$
\boxed{\text{heapsort: }\Theta(n\log n);\quad
\text{quicksort worst case: }\Theta(n^2);\quad
\text{counting sort: }\Theta(n+k).}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Functional programming, data structures and algorithms, procedural programming, and digital hardware](../../../functional-programming-data-structures-and-algorithms-procedural-programming-and-digital-hardware-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

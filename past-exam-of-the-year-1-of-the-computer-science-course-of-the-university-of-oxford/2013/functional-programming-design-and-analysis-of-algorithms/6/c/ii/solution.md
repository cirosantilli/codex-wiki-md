<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Store the [array](../../../../../../array-data-structure.md) as a [binary heap](../../../../../../binary-heap.md) with [min-heap](../../../../../../min-heap.md) order. Build it bottom-up by sifting down internal nodes in reverse order, rather than inserting all $n$ values one at a time. The sum of subtree heights is $O(n)$, so construction costs $\Theta(n)$. Then perform $i$ minimum extractions: output the root, move the last remaining entry to the root, and sift it down to restore the [heap order](../../../../../../heap-order.md).

Each extraction returns the smallest remaining key, so the outputs are the $i$ smallest keys in increasing order. For a heap of current size $s$, an extraction takes $O(\log(s+1))$ time. Hence

$$
T_2(n,i)=O\!\left(n+\sum_{j=0}^{i-1}\log(n-j+1)\right)
=O(n+i\log n).
$$

The tight worst-case bound for this ordinary [binary heap](../../../../../../binary-heap.md) implementation is

$$
\boxed{T_2(n,i)=\Theta(n+i\log n).}
$$

When the extraction term is substantial, worst-case extractions follow root-to-leaf paths of logarithmic length; when $i$ is small, the linear construction already dominates. The bound stays valid at $i=n$, since $\log(n!)=\Theta(n\log n)$. Building by $n$ separate insertions would lose the linear construction bound and is unnecessary.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

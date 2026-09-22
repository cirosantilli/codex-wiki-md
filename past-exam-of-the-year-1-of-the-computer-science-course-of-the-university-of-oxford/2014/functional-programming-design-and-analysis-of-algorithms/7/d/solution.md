<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume $1\le k\le n$. Use [bottom-up heap construction](../../../../../bottom-up-heap-construction.md) to make a [max-heap](../../../../../max-heap.md) of the first $k$ input items. For each subsequent input value $x$, compare it with the root. If $x$ is at least the root, discard it; otherwise replace the root by $x$ and apply [heapify down](../../../../../sift-down.md). Return the final root.

The [loop invariant](../../../../../loop-invariant.md) says the heap contains a multiset of the $k$ smallest values seen so far. It holds after initialization. If $x$ is at least the current largest retained value, the already retained $k$ items are no larger, so discarding $x$ preserves the invariant. If $x$ is smaller, remove one largest retained value and keep $x$ instead; precisely the $k$ smallest values remain. This argument handles equal [integers](../../../../../integer-split.md) by treating repeated occurrences as separate items. At the end,

$$
\boxed{\text{the heap root is the }k\text{th smallest input value}.}
$$

Construction costs $O(k)$; each remaining value uses one comparison and at most one logarithmic repair. Thus the [selection algorithm](../../../../../selection-algorithm.md) has [time complexity](../../../../../time-complexity.md)

$$
\boxed{O\bigl(n+(n-k)\log k\bigr)=O(n\log k)\quad(k\ge2),\qquad O(k)\ \text{space}.}
$$

For $k=1$, the heap is a single running minimum and the time is $O(n)$. The uniform expression $O(n\log(k+1))$ covers that boundary; interpreting the printed $O(n\log k)$ literally at $k=1$ would incorrectly make it zero.

## ↑ Ancestors (12)

1. [D](../d.md)
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

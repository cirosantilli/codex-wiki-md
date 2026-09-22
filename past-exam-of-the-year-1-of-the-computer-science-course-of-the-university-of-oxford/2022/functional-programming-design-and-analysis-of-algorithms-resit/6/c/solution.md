<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This version of [Kadane's algorithm](../../../../../kadane-s-algorithm.md), named for [Joseph Born Kadane](../../../../../joseph-born-kadane.md), permits the empty subsequence. For $j\ge1$, let $E_j$ be the maximum of zero and the weight of a contiguous subsequence ending exactly at position $j$. Let $B_j$ be the best weight anywhere in the first $j$ positions. Use

$$
\boxed{E_0=B_0=0,\qquad E_j=\max(0,E_{j-1}+a_j),\qquad B_j=\max(B_{j-1},E_j).}
$$

A segment ending at $j$ either extends one ending at $j-1$ or starts at $j$; the zero candidate permits discarding a negative predecessor and the empty answer. Any best segment of the first $j$ positions either ends at $j$ or already occurs in the first $j-1$. These two decompositions prove the [dynamic programming](../../../../../dynamic-programming.md) equations by [induction](../../../../../mathematical-induction.md).

Here is an implementation returning endpoints, using zero-based indexing:
```
best_segment(a):
    end_weight = best_weight = 0
    start = best_lo = best_hi = 0
    for j in range(len(a)):
        trial = end_weight + a[j]
        if trial <= 0:
            end_weight = 0
            start = j+1
        else:
            end_weight = trial
        if end_weight > best_weight:
            best_weight = end_weight
            best_lo, best_hi = start, j+1
    return (best_lo, best_hi, best_weight)
```
There is exactly **one addition per input element**, hence $n$ additions and $O(n)$ comparisons. Auxiliary storage is $O(1)$. The all-negative case retains interval $[0,0)$ and weight zero. The example returns $[3,6)$ and weight **8**, hence the desired contiguous subsequence.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Maintain an inclusive interval $[lo,hi]$ with these [recursion invariants](../../../../../recursion-invariant.md): if $lo>0$, then $A[lo]>A[lo-1]$; if $hi<n-1$, then $A[hi]>A[hi+1]$. The original full interval satisfies both conditions vacuously.
```
LocalMaximum(A):
    require length(A) >= 1
    return Peak(0, length(A)-1)

Peak(lo, hi):
    m = floor((lo+hi)/2)
    if m > lo and A[m-1] > A[m]:
        return Peak(lo, m-1)
    if m < hi and A[m+1] > A[m]:
        return Peak(m+1, hi)
    return m
```
In the left-recursion branch, the new right endpoint satisfies $A[m-1]>A[m]$ and the old left boundary is retained. The right-recursion branch is symmetric. Thus both [recursion invariants](../../../../../recursion-invariant.md) persist.

If neither branch is taken, $A[m]$ exceeds its neighbours within the current interval because all entries are distinct. If $m$ is an endpoint of that interval and there is a neighbour outside, the boundary [recursion invariant](../../../../../recursion-invariant.md) supplies the missing strict inequality. Hence the returned index is an **[array local maximum](../../../../../array-local-maximum.md) with respect to the original array**, not just the restricted interval. Every branch shortens the interval, so termination is guaranteed; this also establishes existence, including the singleton case.

Each call performs at most two comparisons, and a recursive interval has at most half as many elements, up to rounding. Thus $T(n)\leq T(\lceil n/2\rceil)+O(1)$ and

$$
\boxed{T(n)=O(1+\log n)}.
$$

The conventional bound is $O(\log n)$ for $n\geq2$, with constant work for a singleton. Distinctness is essential to this proof of a strict local maximum.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

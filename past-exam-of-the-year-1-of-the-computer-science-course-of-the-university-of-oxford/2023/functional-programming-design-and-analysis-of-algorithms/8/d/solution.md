<h1 id="8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Recursively partition into equal halves by rank, keeping the selected median in the lower half:
```
quantiles(A,k):
    if length(A) == k:
        return [maximum(A)]
    p = select the (length(A)/2)-th smallest element of A
    L = all elements of A at most p
    R = all elements of A greater than p
    return quantiles(L,k) followed by quantiles(R,k)
```
All elements are distinct, so both halves have exactly $|A|/2$ elements. Since $|A|/k$ remains a power of two, every internal split occurs at a rank divisible by $k$.

For correctness, the desired ranks in the lower half are $k,2k,\ldots,|A|/2$. In the upper half they are the same local multiples of $k$, shifted by $|A|/2$. These are exactly all desired global ranks. At a leaf of size $k$, its maximum is its sole requested local rank. Induction therefore proves that the output contains every requested [order statistic](../../../../../order-statistic.md), in increasing order, including the original maximum. There is no separate internal-node output of `p`, which would duplicate a rank already supplied by the lower subtree.

Use a worst-case linear-time [selection algorithm](../../../../../selection-algorithm.md) and linear partitioning. The [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md) has

$$
T(n,k)=2T(n/2,k)+\Theta(n)\quad(n>k),\qquad T(k,k)=\Theta(k).
$$

There are $\log_2(n/k)$ internal levels, each with total work $\Theta(n)$, and $n/k$ leaves with total work $\Theta(n)$. Since the source assumes $n/k\geq2$, the running time is

$$
\boxed{\Theta\bigl(n\log(n/k)\bigr)}.
$$

This is [multiselection by balanced rank partitioning](../../../../../multiselection-by-balanced-rank-partitioning.md). In-place selection and partitioning can use the original array; the output has $n/k$ values. The multiselection recursion has depth $O(\log(n/k))$; the selection routine contributes its own auxiliary storage.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [8](../../8.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2023](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

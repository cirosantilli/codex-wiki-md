<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The initial values are **$d_1=0$ and $d_2=1$**: one element cannot move, while two elements must be swapped.

For $n\ge3$, fix one distinguished element, called $n$, and choose its image $j\ne n$, in $n-1$ ways. If $n,j$ form a two-cycle, deleting them leaves an arbitrary [derangement](../../../../../../derangement-of-a-permutation.md) on the other $n-2$ elements, giving $d_{n-2}$ choices.

Otherwise the [permutation cycle](../../../../../../permutation-cycle.md) containing $n$ has length at least three. Remove $n$ from that cycle, joining its predecessor directly to $j$. No fixed point is created because the predecessor is not $j$. This gives a [derangement](../../../../../../derangement-of-a-permutation.md) on $n-1$ elements. Conversely, any such [derangement](../../../../../../derangement-of-a-permutation.md) uniquely recovers the original one by inserting $n$ immediately before $j$ in its cycle. This case contributes $d_{n-1}$ choices for each $j$.

The two cases are disjoint and exhaustive, so the [derangement recurrence](../../../../../../derangement-recurrence.md) is

$$
\boxed{d_n=(n-1)(d_{n-1}+d_{n-2}).}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

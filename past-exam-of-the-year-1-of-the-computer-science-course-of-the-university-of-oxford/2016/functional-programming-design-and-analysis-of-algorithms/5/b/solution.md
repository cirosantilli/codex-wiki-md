<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For one element, return it as both extrema without a comparison. Otherwise compare consecutive pairs once, put each smaller element in a candidate [array](../../../../../array-data-structure.md) $L$ and each larger element in a candidate [array](../../../../../array-data-structure.md) $H$. If one element is unpaired, put it in both candidate arrays. This [simultaneous minimum and maximum](../../../../../simultaneous-minimum-and-maximum.md) construction computes the minimum of $L$ and maximum of $H$ by balanced [divide-and-conquer algorithms](../../../../../divide-and-conquer-algorithm.md): split the candidate array, recursively find the desired extremum in each half, and compare the two returned values. These extremum routines use one comparison per merge and therefore $r-1$ comparisons on $r$ candidates.

Every element excluded from $L$ is at least its paired element, so a global minimum remains in $L$; likewise a global maximum remains in $H$. The recursive extremum routines are correct by [structural induction](../../../../../structural-induction.md). For even $n=2m$, there are $m$ pair comparisons and two searches on $m$ candidates, giving

$$
C(2m)=m+2(m-1)=3m-2.
$$

For odd $n=2m+1\geq3$, there are $m$ pair comparisons and two searches on $m+1$ candidates, giving

$$
C(2m+1)=m+2m=3m.
$$

Together with $C(1)=0$, both cases give

$$
\boxed{C(n)\leq\left\lceil\frac{3n}{2}\right\rceil-2}.
$$

For powers of two, the equivalent direct [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md) returns the ordered pair of extrema for each half, then combines the two minima with one comparison and the two maxima with one comparison. Its base cases must include $C(2)=1$, rather than performing two unnecessary comparisons on a pair. The [recurrence relation](../../../../../recurrence-relation.md) is $C(n)=2C(n/2)+2$ for $n\geq4$, whence $C(n)=3n/2-2$. Arbitrary near-equal splitting without the initial pairing can exceed the desired comparison bound for other values of $n$; the pairing construction above handles every positive size.

## ↑ Ancestors (12)

1. [B](../b.md)
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

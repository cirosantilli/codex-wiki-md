<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume $n\geq1$ and list the elements of $X$ as $a_1,\ldots,a_n$. Define the [partial sums](../../../../../partial-sum.md) $s_j=a_1+\cdots+a_j$ for $1\leq j\leq n$. If one is divisible by $n$, its corresponding nonempty prefix is a suitable $Y$.

Otherwise the $n$ [partial sums](../../../../../partial-sum.md) have remainders in the $n-1$ nonzero [residue classes](../../../../../residue-class.md). The [pigeonhole principle](../../../../../pigeonhole-principle.md) gives $i<j$ with $s_i\equiv s_j\pmod n$. Thus $s_j-s_i=a_{i+1}+\cdots+a_j$ is divisible by $n$, giving a nonempty [subset](../../../../../subset.md) $Y=\{a_{i+1},\ldots,a_j\}$.

Therefore **a nonempty $Y$ exists**. This strengthens the literal assertion, which would otherwise allow the trivial [empty set](../../../../../empty-set.md) with sum zero.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

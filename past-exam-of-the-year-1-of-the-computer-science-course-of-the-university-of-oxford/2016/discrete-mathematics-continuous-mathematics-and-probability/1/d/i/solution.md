<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix one distinguished element $a$ of the $n$-element [set](../../../../../../set-split.md). Every [partition of a set](../../../../../../partition-of-a-set.md) into $l$ blocks belongs to exactly one of two cases. If $\{a\}$ is a block, removing it leaves an $(l-1)$-block [partition of a set](../../../../../../partition-of-a-set.md) of the other $n-1$ elements, giving $S(n-1,l-1)$ possibilities. Otherwise remove $a$ from its block; that block remains nonempty, so the result has $l$ blocks. Conversely choose any of the $S(n-1,l)$ such partitions and insert $a$ in any one of its $l$ blocks. This gives $lS(n-1,l)$ possibilities.

These cases are disjoint and exhaustive, proving the [Stirling numbers of the second kind](../../../../../../stirling-numbers-of-the-second-kind.md) recurrence

$$
\boxed{S(n,l)=lS(n-1,l)+S(n-1,l-1).}
$$

Use $S(0,0)=1$, $S(n,0)=0$ for $n>0$, and $S(n,l)=0$ for $l>n$; these conventions include the boundary cases $n=1$ and $l=1$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

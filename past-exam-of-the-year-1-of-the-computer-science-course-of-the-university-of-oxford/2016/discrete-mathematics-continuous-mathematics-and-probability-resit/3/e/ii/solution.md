<h1 id="3/e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Multiplying the [recurrence relation](../../../../../../recurrence-relation.md) by $n$ removes the average:

$$
nT(n)=\sum_{i=0}^{n-1}T(i)+n^2.
$$

For $n\geq2$, subtract the same identity at $n-1$:

$$
nT(n)-(n-1)T(n-1)=T(n-1)+n^2-(n-1)^2.
$$

Rearranging gives $T(n)=T(n-1)+2-1/n$. This also holds at $n=1$, because the original [recurrence relation](../../../../../../recurrence-relation.md) gives $T(1)=1$ and $T(0)=0$. Summing the differences therefore yields

$$
\boxed{T(n)=2n-H_n=O(n)},\qquad H_n=\sum_{j=1}^{n}\frac1j,\quad H_0=0.
$$

Here $H_n$ is a [harmonic number](../../../../../../harmonic-number.md). Since $H_n\leq n$, we have $n\leq T(n)\leq2n$ for $n\geq1$, also establishing $\Theta(n)$ in [big theta notation](../../../../../../big-theta-notation.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [E](../../e.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

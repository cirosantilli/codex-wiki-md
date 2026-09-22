<h1 id="3/f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We prove the stronger explicit bound $n!\leq n^n/2^{n-1}$ by [mathematical induction](../../../../../../mathematical-induction.md). The case $n=1$ is equality. The [binomial theorem](../../../../../../binomial-theorem.md) gives $(1+1/n)^n\geq1+n/n=2$, so $(n+1)^n\geq2n^n$. Consequently the [induction hypothesis](../../../../../../induction-hypothesis.md) yields

$$
(n+1)!\leq\frac{(n+1)n^n}{2^{n-1}}\leq\frac{(n+1)^{n+1}}{2^n}.
$$

Therefore **$n!=O(n^n/2^n)$**, with constant $2$ and threshold $1$.

The second bound is **asymptotically tighter**. Using $n\leq2^n$,

$$
\frac{n^n/2^n}{2^{n^2}}=\left(\frac{n}{2^{n+1}}\right)^n\leq2^{-n}\longrightarrow0.
$$

Thus its bounding function is negligible relative to the first in [little o notation](../../../../../../little-o-notation.md); this compares the bounds without needing [Stirling's formula](../../../../../../stirling-formula.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [F](../../f.md)
3. [3](../../../3.md)
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

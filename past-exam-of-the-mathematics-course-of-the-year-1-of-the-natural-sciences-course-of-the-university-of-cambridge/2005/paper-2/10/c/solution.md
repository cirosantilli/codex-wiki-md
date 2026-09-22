<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $p>0$, the partial sums are increasing and bounded above by $1+1/p$. The [monotone convergence theorem for sequences](../../../../../bounded-monotone-sequence-theorem.md) therefore proves convergence to a finite sum $S(p)$. Passing to the limit $N\to\infty$ in the two bounds gives

$$
\frac1p\leq S(p)\leq\frac1p+1,\qquad1\leq pS(p)\leq1+p.
$$

The [squeeze theorem](../../../../../squeeze-theorem.md) now yields

$$
\boxed{\lim_{p\downarrow0}p\sum_{n=1}^\infty n^{-1-p}=1.}
$$

Since $S(p)=\zeta(1+p)$, this is the [real-axis singular limit of the Riemann zeta function at one](../../../../../real-axis-singular-limit-of-the-riemann-zeta-function-at-one.md). The limiting sum is taken at fixed $p$ before sending $p$ to zero; setting $p=0$ inside the convergent-series argument would instead give the divergent harmonic series.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

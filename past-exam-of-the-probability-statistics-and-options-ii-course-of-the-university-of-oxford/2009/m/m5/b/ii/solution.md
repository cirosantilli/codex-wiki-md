<h1 id="m/m5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $j\ge1$ the only entrance is from $j-1$, so stationarity requires $\pi_j=\pi_{j-1}\lambda/j$. [Induction](../../../../../../mathematical-induction.md) gives $\pi_j=\pi_0\lambda^j/j!$, and normalization using the exponential series gives $\pi_0=e^{-\lambda}$. Hence

$$
\boxed{\pi_j=e^{-\lambda}\frac{\lambda^j}{j!},\qquad j=0,1,\ldots.}
$$

The remaining zero-state equation also holds: $\sum_i\pi_i\lambda/(i+1)=e^{-\lambda}(e^\lambda-1)=1-\pi_0$, so $\sum_i\pi_i(1-\lambda/(i+1))=\pi_0$. Thus this normalized [Poisson law](../../../../../../poisson-distribution.md) really is stationary, not just a solution of the positive-state equations. Irreducibility makes the stationary probability law unique.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [M5](../../../m5.md)
4. [M](../../../../m.md)
5. [2009](../../../../../2009-split.md)
6. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options II course of the University of Oxford](../../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)

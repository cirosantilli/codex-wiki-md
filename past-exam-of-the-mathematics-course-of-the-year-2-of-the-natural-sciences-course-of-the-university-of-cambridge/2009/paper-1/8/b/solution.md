<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the analytic solution as $w(z)=\sum_{n\geq0}a_nz^n$. The constant term in the differential equation gives $a_1=0$, and matching the coefficient of $z^{n+1}$ gives

$$
(n+2)^2a_{n+2}+4a_n=0,\qquad n\geq0.
$$

All odd coefficients therefore vanish; $a_2=-a_0$ and $a_4=a_0/4$. The first three nonzero terms are

$$
\boxed{w(z)=a_0\left(1-z^2+\frac{z^4}{4}+O(z^6)\right).}
$$

In full, $a_{2j}=(-1)^ja_0/(j!)^2$, so $w=a_0J_0(2z)$, a [Bessel function of the first kind](../../../../../bessel-function-of-the-first-kind.md). The [ratio test](../../../../../ratio-test.md) proves convergence for every complex $z$. The other independent solution has a logarithmic singularity at zero and does not satisfy the analyticity requirement.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

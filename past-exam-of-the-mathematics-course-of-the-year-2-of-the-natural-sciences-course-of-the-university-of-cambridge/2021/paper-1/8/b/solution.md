<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the [Frobenius solution](../../../../../frobenius-solution.md), differentiate term by term:

$$
y'=\sum_{n\geq0}(n+\sigma)a_nx^{n+\sigma-1},\qquad y''=\sum_{n\geq0}(n+\sigma)(n+\sigma-1)a_nx^{n+\sigma-2}.
$$

The unshifted terms in the equation have coefficient $[4(n+\sigma)(n+\sigma-1)-4(n+\sigma)+3]a_n$. The extra factors of $x$ give the shifted contribution $[4(n+\sigma)(n+\sigma-1)+1]a_nx^{n+\sigma+1}$. Equating the coefficient of $x^{k+\sigma}$ for $k\geq1$ gives the [linear recurrence relation](../../../../../linear-recurrence-relation.md)

$$
\boxed{[4(k+\sigma)^2-8(k+\sigma)+3]a_k+[4(k+\sigma-1)(k+\sigma-2)+1]a_{k-1}=0.}
$$

Factoring both coefficients is especially useful:

$$
\boxed{(2k+2\sigma-3)\big[(2k+2\sigma-1)a_k+(2k+2\sigma-3)a_{k-1}\big]=0.}
$$

The separate lowest-power equation is $(4\sigma^2-8\sigma+3)a_0=0$. Do not cancel $2k+2\sigma-3$ when it vanishes: that is the possible [undetermined coefficient at Frobenius resonance](../../../../../undetermined-coefficient-at-frobenius-resonance.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

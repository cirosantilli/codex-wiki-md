<h1 id="7/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

With independent samples and finite [variance](../../../../../variance-split.md), [Monte Carlo integration](../../../../../monte-carlo-integration.md) has a root-mean-square stochastic error proportional to **$N^{-1/2}$**. The estimated [standard error](../../../../../standard-error.md) measures that random sampling uncertainty; it is not a deterministic bound.

For a sufficiently smooth one-dimensional [integrand](../../../../../integrand.md), the composite [trapezoidal rule](../../../../../trapezoidal-rule.md) has error

$$
I-T_n=-\frac{(b-a)^3}{12n^2}f''(\xi)
$$

for some $\xi\in(a,b)$, hence **$O(n^{-2})$**. It is normally much more efficient in one dimension. The stated continuity assumption alone guarantees convergence, but does not guarantee this second-order rate; bounded second derivatives are an additional assumption.

The dimensional advantage is different: a tensor grid with $N$ total points in $d$ dimensions has only about $N^{1/d}$ points per direction and typically error $O(N^{-2/d})$. The Monte Carlo exponent remains $-1/2$, although its [variance](../../../../../variance-split.md) prefactor can still deteriorate with dimension. This explains why the stochastic method becomes attractive for high-dimensional integrals.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [7](../../7.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2022](../../../split.md)
5. [Past exam of the chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Chemistry course of the year 4 of the natural sciences course of the University of Cambridge](../../../../../chemistry-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

<h1 id="o/o4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under [independence](../../../../../independent-random-variables.md), the log [likelihood function](../../../../../likelihood-function.md) separates:

$$
\ell(\alpha,\beta)=\sum_i n_{i.}\log\alpha_i+
\sum_j n_{.j}\log\beta_j.
$$

Maximizing the two terms over their respective [probability](../../../../../probability.md) simplices, by the same [Lagrange multiplier](../../../../../lagrange-multiplier.md) argument as in part (a), gives

$$
\widehat\alpha_i=\frac{n_{i.}}N,\qquad
\widehat\beta_j=\frac{n_{.j}}N.
$$

Therefore the constrained [maximum-likelihood estimates](../../../../../maximum-likelihood-estimation-split.md) are

$$
\boxed{\widehat\theta_{ij}^{\,0}=\frac{n_{i.}n_{.j}}{N^2}.}
$$

The associated fitted cell counts are $E_{ij}=N\widehat\theta_{ij}^{\,0}=n_{i.}n_{.j}/N$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [O4](../../o4.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

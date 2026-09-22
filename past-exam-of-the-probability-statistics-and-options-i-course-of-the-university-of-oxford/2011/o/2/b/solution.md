<h1 id="o/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $S=\sum_iX_i$, the ratio of the two sample [likelihood functions](../../../../../likelihood-function.md) is

$$
\frac{L(\mu_1)}{L(\mu_0)}
=e^{-n(\mu_1-\mu_0)}\left(\frac{\mu_1}{\mu_0}\right)^S.
$$

For $0<\mu_0<\mu_1$ it is strictly increasing in $S$. The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) therefore selects an upper tail:

$$
\boxed{C=\{\mathbf x:\textstyle\sum_i x_i\geq k\}.}
$$

Under the null, $S\sim\operatorname{Poisson}(n\mu_0)$, so choose $k$ with this upper-tail probability at most $\alpha$. If exact size $\alpha$ is required, randomize at the adjacent boundary value as needed. The rejection rule is the same for every $\mu_1>\mu_0$, giving a [uniformly most powerful test](../../../../../uniformly-most-powerful-test.md) for the one-sided alternative.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

<h1 id="s/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For unknown normalization constants, use [self-normalized importance sampling](../../../../../self-normalized-importance-sampling.md) with $\tilde w=\tilde p/\tilde q$:

$$
\boxed{\tilde\mu_N=
\frac{\sum_i\tilde w(X_i)f(X_i)}{\sum_i\tilde w(X_i)}.}
$$

Under the same support condition, $E_q\tilde w=Z_p/Z_q>0$ and $E_q[\tilde w f]=(Z_p/Z_q)\mu$. Moreover $E_q|\tilde w f|=(Z_p/Z_q)E_p|f|<\infty$, by [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and the supplied $E_pf^2<\infty$. The [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) applies to numerator and denominator sample averages. Their ratio tends almost surely, hence in probability, to $\mu$. If a finite sample happens to give zero denominator, it can be assigned an arbitrary value; this does not affect the eventual almost sure limit. The ratio estimator is generally biased at finite $N$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [S](../../../s.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options I course of the University of Oxford](../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

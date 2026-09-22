<h1 id="o/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Neyman-Pearson lemma](../../../../neyman-pearson-lemma.md) says that for testing a simple null density $f_0$ against a simple alternative $f_1$, a size-$\alpha$ test that rejects for the largest values of $f_1/f_0$ is most powerful. Randomization on a likelihood-ratio boundary can be used to achieve the exact size.

The source writes the same $\lambda_0$ in both hypotheses but immediately introduces $\lambda_1>\lambda_0$. Use the intended alternative $\lambda=\lambda_1$. If read literally as two identical hypotheses, there is no such distinct alternative to test.

For Weibull shape two, the sample likelihood is proportional to

$$
\lambda^{-2n}\exp\left(-\frac1{\lambda^2}\sum_iX_i^2\right).
$$

Thus

$$
\frac{L(\lambda_1)}{L(\lambda_0)}
=\left(\frac{\lambda_0}{\lambda_1}\right)^{2n}
\exp\left[\left(\lambda_0^{-2}-\lambda_1^{-2}\right)\sum_iX_i^2\right],
$$

which is increasing in $S=\sum_iX_i^2$. The most powerful critical region is therefore

$$
\boxed{S\geq C,\qquad
\mathbb P_{\lambda_0}(S\geq C)=\alpha.}
$$

Indeed, $2S/\lambda_0^2\sim\chi^2_{2n}$, so $C=(\lambda_0^2/2)q_{2n,1-\alpha}$. The critical value depends only on the null and size, not on the chosen larger alternative. Hence the same test is **uniformly most powerful for $\lambda>\lambda_0$**, and in particular for the printed restricted range $\lambda>\lambda_1$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [O](../../o.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

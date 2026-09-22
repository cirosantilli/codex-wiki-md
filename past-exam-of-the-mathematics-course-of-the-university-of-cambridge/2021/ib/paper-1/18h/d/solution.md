<h1 id="18h/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The normalized density is

$$
f_\theta(x)=(\theta+1)x^\theta\mathbf1_{(0,1)}(x).
$$

For $\theta=1$ against $\theta=0$, the sample likelihood ratio is

$$
\frac{L(1)}{L(0)}
=2^n\prod_{i=1}^nX_i
=2^ne^{-S},
\qquad
S=-\sum_{i=1}^n\log X_i.
$$

It is strictly decreasing in $S$. Under $H_0$, parts (a) and (b) give

$$
S\sim\Gamma(n,1).
$$

If $q_\alpha$ is the lower $\alpha$-quantile of this gamma distribution, the [Neyman-Pearson lemma](../../../../../../neyman-pearson-lemma.md) gives the most powerful size-$\alpha$ critical region

$$
\boxed{S\leq q_\alpha}.
$$

For any fixed $\theta>0$,

$$
\frac{L(\theta)}{L(0)}
=(\theta+1)^ne^{-\theta S}
$$

is again strictly decreasing in the same statistic $S$. Thus the same critical region is most powerful against every $\theta>0$ and is consequently a [uniformly most powerful test](../../../../../../uniformly-most-powerful-test.md) of $H_0:\theta=0$ against $H_1:\theta>0$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

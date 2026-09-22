<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [quota share reinsurance](../../../../../../quota-share-reinsurance.md) the insurer retains the same fraction of each claim, so

$$
\boxed{g(x)=\alpha x.}
$$

The annual retained loss is consequently $T_I=\alpha T$. Each transformed risk severity has [probability density function](../../../../../../probability-density-function.md) $f_i(y/\alpha)/\alpha$ for $y>0$. The mixed transformed severity, with the same weights $\lambda_i/(\lambda_1+\lambda_2)$, still gives a [compound Poisson distribution](../../../../../../compound-poisson-distribution.md). Scaling the [expected value](../../../../../../expected-value.md) and [variance](../../../../../../variance-split.md) gives

$$
\boxed{\mathbb ET_I=\alpha\sum_{i=1}^2\lambda_i\mu_i,\qquad
\operatorname{Var}(T_I)=\alpha^2\sum_{i=1}^2\lambda_i(\sigma_i^2+\mu_i^2).}
$$

This agrees with the general retained-claim formulas because $\mathbb E g(X_i)=\alpha\mu_i$ and $\mathbb E[g(X_i)^2]=\alpha^2(\sigma_i^2+\mu_i^2)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

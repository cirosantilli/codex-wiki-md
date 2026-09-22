<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $f=f_0/C_f$ and $g=g_0/C_g$, where $f_0,g_0$ are known nonnegative kernels. If both constants are known, the ordinary weight is $(C_g/C_f)f_0/g_0$. If their ratio is unknown, use [self-normalized importance sampling](../../../../../../self-normalized-importance-sampling.md):

$$
\boxed{\widehat\mu_{\mathrm{SN}}
=\frac{\sum_i\theta(x_i)f_0(x_i)/g_0(x_i)}{\sum_i f_0(x_i)/g_0(x_i)}.}
$$

Indeed, under the normalized proposal law,

$$
\mathbb E_g\!\left[\frac{f_0(X)}{g_0(X)}\theta(X)\right]
=\frac{C_f}{C_g}\mu,
\qquad
\mathbb E_g\!\left[\frac{f_0(X)}{g_0(X)}\right]=\frac{C_f}{C_g}.
$$

The [strong law of large numbers](../../../../../../strong-law-of-large-numbers.md) makes their empirical ratio converge to $\mu$, provided the numerator is absolutely [integrable](../../../../../../integrability.md) and $0<C_f,C_g<\infty$. Multiplicative constants cancel, whether the unknown one belongs to the target, proposal, or both. Unlike the estimator in part (i), this ratio is generally biased at finite sample size. Exact sampling from $g$ is still presumed; knowing only an unnormalized proposal does not itself supply a sampler.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

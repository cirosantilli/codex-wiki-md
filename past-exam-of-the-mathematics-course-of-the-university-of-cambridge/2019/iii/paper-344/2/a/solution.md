<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\mu_j=\delta F/\delta p_j$ and $\int=\int_{t_1}^{t_2}dt\int d\mathbf r$. Eliminating the noise gives $f=\dot p+\Gamma\mu$. The [Onsager--Machlup path probability](../../../../../../onsager-machlup-path-probability.md) is therefore

$$
\boxed{P_F[p]=\mathcal K[p]\exp\left[-\frac1{2\sigma^2}\int|\dot p+\Gamma\mu|^2\right],\qquad
P_B[p]=\mathcal K[p]\exp\left[-\frac1{2\sigma^2}\int|-\dot p+\Gamma\mu|^2\right].}
$$

These are conditional path densities given the corresponding starting configuration. For a time-even [vector order parameter](../../../../../../vector-order-parameter.md), reversal reads the configurations backward, changes $\dot p$ to $-\dot p$, and keeps $\mu$ unchanged on each corresponding configuration.

The two [Gaussian white noise](../../../../../../gaussian-white-noise.md) measures have the same normalization. With a common midpoint discretization, the noise-to-path Jacobian also agrees under reversal by [time-reversal invariance of a path Jacobian](../../../../../../time-reversal-invariance-of-a-path-jacobian.md). The common factor $\mathcal K[p]$ may include that path-dependent Jacobian; it need not be a universal constant. This makes the shared-factor assertion precise while leaving the requested ratio unaffected.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

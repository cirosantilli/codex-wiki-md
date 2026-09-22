<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Neyman-Pearson lemma](../../../../../../neyman-pearson-lemma.md) says that for simple hypotheses with densities $f_0,f_1$, a size-$\alpha$ test that rejects where $f_1/f_0>k$ and accepts where $f_1/f_0<k$, with possible randomization on equality to attain size $\alpha$, is most powerful among all tests of size at most $\alpha$. To prove it, let $\varphi^*$ be this test and $\varphi$ any competing test. Pointwise,

$$
(\varphi^*-\varphi)(f_1-kf_0)\geq0.
$$

After integration,

$$
\mathbb E_1\varphi^*-\mathbb E_1\varphi
\geq k(\mathbb E_0\varphi^*-\mathbb E_0\varphi)\geq0,
$$

which proves maximal power.

For the exponential sample, with $S=\sum_iX_i=n\overline X$,

$$
\frac{L(\lambda_1)}{L(\lambda_0)}
=\left(\frac{\lambda_1}{\lambda_0}\right)^n
\exp\bigl((\lambda_0-\lambda_1)S\bigr).
$$

Since $\lambda_1<\lambda_0$, this ratio is increasing in $S$. The [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) therefore rejects for large $\overline X$:

$$
\boxed{R_\alpha=\{\overline X>c_\alpha\},
\qquad
1-G_{n,\lambda_0}(nc_\alpha)=\alpha},
$$

where $G_{n,\lambda}$ is the distribution function of the rate-parameterized [Gamma distribution](../../../../../../gamma-distribution.md) $\Gamma(n,\lambda)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

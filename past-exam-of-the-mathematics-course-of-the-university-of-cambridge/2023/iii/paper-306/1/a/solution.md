<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md) of each component of the [string embedding map](../../../../../../string-embedding-map.md) is the [wave equation](../../../../../../wave-equation-split.md) $(\partial_\tau^2-\partial_\sigma^2)X^\mu=0$. Its left- and right-moving solutions are identified by the endpoint [Neumann boundary conditions](../../../../../../neumann-boundary-condition.md), so the resulting [open-string mode expansion](../../../../../../open-string-mode-expansion.md) is

$$
X^\mu(\sigma,\tau)=x^\mu+2\alpha'p^\mu\tau
+i\sqrt{2\alpha'}\sum_{n\ne0}\frac{\alpha_n^\mu}{n}
e^{-in\tau}\cos(n\sigma),
\qquad \alpha_{-n}^\mu=(\alpha_n^\mu)^\dagger.
$$

Indeed, the [Fourier cosine series](../../../../../../fourier-cosine-series.md) makes $\partial_\sigma X^\mu$ vanish at $\sigma=0,\pi$. The canonical momentum density is $\Pi_\mu=(2\pi\alpha')^{-1}\dot X_\mu$. Imposing the equal-time [canonical commutation relations](../../../../../../canonical-commutation-relation.md) $[X^\mu(\sigma),\Pi_\nu(\sigma')]=i\delta^\mu_\nu\delta(\sigma-\sigma')$ gives the [covariant quantization of the bosonic string](../../../../../../covariant-quantization-of-the-bosonic-string.md)

$$
[x^\mu,p^\nu]=i\eta^{\mu\nu},
\qquad
[\alpha_m^\mu,\alpha_n^\nu]=m\,\delta_{m+n,0}\eta^{\mu\nu},
\qquad
[x,x]=[p,p]=0,
$$

with $\alpha_0^\mu=\sqrt{2\alpha'}p^\mu$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

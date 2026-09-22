<h1 id="31l/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a fixed sample $x_{1:n}$ and independent Rademacher signs $\sigma_i$,

$$
\widehat{\mathcal R}(H(x_{1:n}))
=\mathbb E_\sigma\sup_{h\in H}\frac1n\sum_{i=1}^n\sigma_i h(x_i).
$$

The [Rademacher complexity](../../../../../../rademacher-complexity.md) is

$$
\mathcal R_n(H)=\mathbb E_{X_{1:n}}\widehat{\mathcal R}(H(X_{1:n})).
$$

The contraction lemma says that if each $\psi_i$ is $L$-Lipschitz and $\psi_i(0)=0$, then

$$
\mathbb E_\sigma\sup_{h\in H}\frac1n\sum_i\sigma_i\psi_i(h(x_i))
\leq L\widehat{\mathcal R}(H(x_{1:n})).
$$

Subtracting constants handles maps not vanishing at zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31L](../../31l.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

By [Donald's identity](../../../../../../donald-s-identity.md), the objective equals

$$
\sum_jp_jD(\omega_j\|\rho)=\sum_jp_jD(\omega_j\|\overline\omega)+D(\overline\omega\|\rho).
$$

The [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md) makes the last term at least zero, with equality exactly when $\rho=\overline\omega$. Hence the unique minimizing [density operator](../../../../../../density-matrix.md) is the ensemble average and

$$
\min_\rho\sum_jp_jD(\omega_j\|\rho)
=\sum_jp_jD(\omega_j\|\overline\omega)
=S(\overline\omega)-\sum_jp_jS(\omega_j).
$$

For the [classical-quantum state](../../../../../../classical-quantum-state.md) $\sigma_{XB}$, its marginal on $X$ has entropy $H(p)$, its marginal on $B$ is $\overline\omega$, and its joint entropy is $H(p)+\sum_jp_jS(\omega_j)$. Substituting in the definition of [quantum mutual information](../../../../../../quantum-mutual-information.md) gives

$$
\boxed{\min_\rho\sum_jp_jD(\omega_j\|\rho)
=\chi(\{p_j,\omega_j\})=I(X:B)_\sigma,\qquad\rho_{\min}=\overline\omega}.
$$

This is the [relative-entropy barycenter of a quantum ensemble](../../../../../../relative-entropy-barycenter-of-a-quantum-ensemble.md): the average state minimizes mean distinguishability from the ensemble. Its minimal value is exactly the [Holevo quantity](../../../../../../holevo-quantity.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

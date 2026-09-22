<h1 id="4/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Assume the displayed variational minimizer exists and $K:U\to V$ is bounded and linear. The smooth data-fidelity term and the [subdifferential sum rule](../../../../../../subdifferential-sum-rule.md) give

$$
p_\alpha=\frac1\alpha K^*(f^\delta-Ku_\alpha)\in\partial J(u_\alpha).
$$

Use the supplied [source condition in variational regularization](../../../../../../source-condition-in-variational-regularization.md) $p^\dagger=K^*w\in\partial J(u^\dagger)$. Put $e=f^\delta-f$ and $q=K(u_\alpha-u^\dagger)$, so $\|e\|\leq\delta$. By the [symmetric Bregman distance](../../../../../../symmetric-bregman-distance.md) identity,

$$
\alpha D_J^{\mathrm{sym}}(u_\alpha,u^\dagger)=\langle e-q-\alpha w,q\rangle=\frac14\|e-\alpha w\|^2-\left\|q-\frac{e-\alpha w}{2}\right\|^2.
$$

Dropping the last square and using $\|e-\alpha w\|^2\leq2\|e\|^2+2\alpha^2\|w\|^2$ proves the [source-condition estimate for symmetric Bregman distance](../../../../../../source-condition-estimate-for-symmetric-bregman-distance.md):

$$
\boxed{D_J^{\mathrm{sym}}(u_\alpha,u^\dagger)\leq\frac{\|e-\alpha w\|^2}{4\alpha}\leq\frac{\delta^2}{2\alpha}+\frac\alpha2\|w\|_V^2.}
$$

The source condition also makes $u^\dagger$ a $J$-minimizing exact solution: for $Ku=f$, its [subgradient](../../../../../../subgradient.md) inequality has zero pairing with $u-u^\dagger$. Existence of $u_\alpha$ is not implied by properness and lower semicontinuity alone; it is a hypothesis when no coercivity/compactness condition is provided.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [4](../../4.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

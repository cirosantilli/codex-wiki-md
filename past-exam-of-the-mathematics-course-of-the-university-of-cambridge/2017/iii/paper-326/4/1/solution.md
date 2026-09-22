<h1 id="4/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a convex functional $J:U\to\mathbb R\cup\{+\infty\}$ on a real [Banach space](../../../../../../banach-space-split.md), its [subdifferential](../../../../../../subdifferential.md) at $v$ is empty unless $J(v)$ is finite; otherwise

$$
\boxed{\partial J(v)=\{p\in U^*:J(u)\geq J(v)+\langle u-v,p\rangle\ \text{for all }u\in U\}.}
$$

Given $p_v\in\partial J(v)$, the [Bregman distance](../../../../../../bregman-divergence.md) is

$$
\boxed{D_J^{p_v}(u,v)=J(u)-J(v)-\langle u-v,p_v\rangle\geq0.}
$$

It can be infinite if $J(u)$ is infinite. If $J$ is differentiable at $v$, the choice is its derivative; otherwise the base [subgradient](../../../../../../subgradient.md) must be specified. Given also $p_u\in\partial J(u)$, add both directional distances to obtain the [symmetric Bregman distance](../../../../../../symmetric-bregman-distance.md)

$$
\boxed{D_J^{\mathrm{sym}}(u,v)=D_J^{p_v}(u,v)+D_J^{p_u}(v,u)=\langle p_u-p_v,u-v\rangle.}
$$

The symmetric version here is the sum, not half the sum. These nonnegative quantities are not generally metrics and can vanish at distinct points.

## ↑ Ancestors (11)

1. [1](../1.md)
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

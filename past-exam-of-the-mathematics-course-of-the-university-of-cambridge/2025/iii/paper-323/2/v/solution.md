<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

At the proposed boundary $p_0=1/(d+1)$, the identity from part (iv) yields

$$
\rho_{p_0}
=\frac{d}{d+1}\sigma
+\frac1{d+1}\frac Dd.
$$

Both $\sigma$ and $D/d$ are [convex combinations](../../../../../../convex-combination.md) of [product states](../../../../../../product-state.md), so $\rho_{p_0}$ is a [separable quantum state](../../../../../../separable-quantum-state.md). For $0\leq p\leq p_0$, the state $\rho_p$ is a convex combination of $\rho_{p_0}$ and the maximally mixed product state $I/d^2$, and is therefore separable.

For the converse, the [partial transpose](../../../../../../partial-transpose.md) of the maximally entangled projector is $F/d$, where $F$ is the [swap operator](../../../../../../swap-operator.md). Therefore

$$
\rho_p^{T_B}=\frac pdF+\frac{1-p}{d^2}I.
$$

On the antisymmetric subspace, $F$ has eigenvalue $-1$, so the corresponding eigenvalue of $\rho_p^{T_B}$ is

$$
\frac{1-p}{d^2}-\frac pd,
$$

which is negative exactly when $p>1/(d+1)$. The [positive partial transpose criterion](../../../../../../positive-partial-transpose-criterion.md) then proves that $\rho_p$ is entangled. Thus

$$
\boxed{\rho_p\text{ is separable exactly when }p\leq\frac1{d+1}}.
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

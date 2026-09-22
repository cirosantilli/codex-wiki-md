<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $J_0$ be the standard [complex structure](../../../../../../complex-structure.md) on $\mathbb R^{2n}$, let $\omega_0$ be the standard [symplectic form](../../../../../../symplectic-form.md), and let $g_0$ be the Euclidean [inner product](../../../../../../inner-product.md). They satisfy

$$
g_0(u,v)=\omega_0(u,J_0v),
\qquad
\omega_0(u,v)=g_0(J_0u,v).
$$

The [two-out-of-three property for unitary structures](../../../../../../two-out-of-three-property-for-unitary-structures.md) says that a real linear map preserving any two of these structures preserves the third. In terms of the corresponding [matrix groups](../../../../../../matrix-group.md),

$$
GL(n,\mathbb C)\cap Sp(2n,\mathbb R)
=Sp(2n,\mathbb R)\cap O(2n)
=O(2n)\cap GL(n,\mathbb C)
=U(n).
$$

For example, if $A$ preserves $J_0$ and $\omega_0$, then

$$
g_0(Au,Av)=\omega_0(Au,J_0Av)
=\omega_0(Au,AJ_0v)=g_0(u,v),
$$

so $A$ preserves $g_0$. If it preserves $J_0$ and $g_0$, the second displayed identity shows that it preserves $\omega_0$. Finally, $J_0$ is uniquely determined by $g_0(J_0u,v)=\omega_0(u,v)$, so preservation of $g_0$ and $\omega_0$ implies $AJ_0=J_0A$. The common intersection is therefore the [unitary group](../../../../../../unitary-group.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 146](../../../paper-146-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

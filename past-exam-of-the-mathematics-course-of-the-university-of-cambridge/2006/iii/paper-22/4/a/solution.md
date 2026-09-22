<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use anti-Hermitian $SU(2)$ [vector-bundle curvature](../../../../../../curvature-form.md) and the fundamental [matrix trace](../../../../../../matrix-trace.md), so

$$
k(E)=c_2(E)[X]=\frac1{8\pi^2}\int_X\operatorname{Tr}(F\wedge F)
$$

is an integer on a closed oriented four-manifold. The supplied formula's phrase “extending $W$” is a typographical error in the original PDF: the connection extends the boundary connection $\nabla$. An extension exists, for example on the trivial bundle over $B^4$, by extending a boundary connection through a collar and cutting it off farther inside.

For well-definedness, glue two choices $W_0$ and $-W_1$ along their identified boundary bundles. Connections may be made product connections on a collar while keeping their boundary values, and the transgression identity below shows that this does not alter the relevant integral. The glued bundle over the resulting closed four-manifold has an integer [Second Chern number](../../../../../../second-chern-number.md). Therefore the two extension integrals differ by an integer, proving **the value of $\operatorname{CS}$ is independent of all choices in $\mathbb R/\mathbb Z$**. In particular, different extensions on one fixed bundle with the same boundary value have zero difference by transgression and [Stokes theorem](../../../../../../stokes-theorem.md).

To compute the derivative, extend the boundary variation $a$ to an adjoint-valued one-form $\widetilde a$ on $W$ and set $\widetilde\nabla_t=\widetilde\nabla+t\widetilde a$. The [vector-bundle curvature](../../../../../../curvature-form.md) derivative is $\dot F=d_{\widetilde\nabla}\widetilde a$. Invariance of the trace and the [Bianchi identity](../../../../../../bianchi-identity.md) give

$$
\begin{aligned}
\left.\frac d{dt}\right|_0\operatorname{Tr}(F_t\wedge F_t)
&=2\operatorname{Tr}(d_{\widetilde\nabla}\widetilde a\wedge F)\\
&=2d\operatorname{Tr}(\widetilde a\wedge F).
\end{aligned}
$$

The second equality follows from the covariant product rule; its other term contains $d_{\widetilde\nabla}F=0$. Integrating and applying [Stokes theorem](../../../../../../stokes-theorem.md), with the given boundary orientation, yields

$$
\boxed{\left.\frac d{dt}\right|_0\operatorname{CS}(\nabla+ta)
=\frac1{4\pi^2}\int_{S^3}\operatorname{Tr}(F_\nabla\wedge a).}
$$

This derivative means the derivative of any local real lift of the circle-valued functional; changing that lift by an integer changes no derivative.

If a [bundle gauge transformation](../../../../../../unitary-bundle-gauge-transformation.md) $u$ extends to $\widetilde u$ on $W$, use $\widetilde u^{-1}\widetilde\nabla\widetilde u$ as the extension of the transformed boundary connection. [Vector-bundle curvature](../../../../../../curvature-form.md) is conjugated, so its trace square is unchanged pointwise. **$\operatorname{CS}(u\cdot\nabla)=\operatorname{CS}(\nabla)$.** This proof even preserves the chosen extension's real integral, before reducing modulo integers. The local [Chern-Simons three-form](../../../../../../chern-simons-3-form.md) transgresses the same characteristic form and is the boundary expression used in the compactness argument below.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

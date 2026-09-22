<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**False even when both base and fibre are closed and oriented.** Take the [Hopf fibration](../../../../../../hopf-fibration.md) $h:S^3\to S^2$, and define the smooth [fiber bundle](../../../../../../fiber-bundle-split.md) $p:S^3\times S^1\to S^2$ by $p(x,\theta)=h(x)$. Its local trivializations are the Hopf trivializations times $S^1$, and its fibre is $S^1\times S^1=T^2$.

The [Künneth theorem](../../../../../../kunneth-theorem.md) for [cohomology](../../../../../../cohomology-split.md) over a field says $H^k(A\times B;\mathbb R)=\bigoplus_{i+j=k}H^i(A;\mathbb R)\otimes H^j(B;\mathbb R)$ for these compact manifolds. Here it gives $H^2(S^3\times S^1;\mathbb R)=0$. If a [symplectic form](../../../../../../symplectic-form.md) $\omega$ existed on this closed four-manifold, it would be exact, $\omega=d\eta$. Since $d\omega=0$,

$$
\int_{S^3\times S^1}\omega\wedge\omega
=\int_{S^3\times S^1}d(\eta\wedge\omega)=0
$$

by [Stokes theorem](../../../../../../stokes-theorem.md). But $\omega^2$ is a positive volume form in the [symplectic orientation](../../../../../../symplectic-orientation.md), so its integral is positive. This contradiction proves the claim fails. The mere bundle structure does not ensure that a fibrewise area class extends to the total space.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

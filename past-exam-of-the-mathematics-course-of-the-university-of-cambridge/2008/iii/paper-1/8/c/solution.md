<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A closed subspace invariant under a [star-algebra](../../../../../../star-algebra.md) is reducing, since it is invariant under every adjoint as well. Thus the [orthogonal projections](../../../../../../orthogonal-projection.md) $P_1,P_2$ onto $H_1,H_2$ commute with $M$. Consider the bounded intertwiner

$$
T=(I-P_2)|_{H_1}:H_1\longrightarrow H_2^\perp.
$$

Its [kernel](../../../../../../kernel-of-a-linear-map.md) is $H_1\cap H_2$, so its initial polar space is

$$
K_1=H_1\cap(H_1\cap H_2)^\perp.
$$

Its closed range is

$$
K_2=\overline{H_1+H_2}\cap H_2^\perp.
$$

For the inclusion from left to right, $(I-P_2)h_1=h_1-P_2h_1$ lies in $H_1+H_2$ and is orthogonal to $H_2$. Conversely, approximate any $z$ in the displayed $K_2$ by $h_{1,n}+h_{2,n}$ and apply $I-P_2$. The images converge to $z$ and equal $Th_{1,n}$, proving the reverse inclusion after [closure](../../../../../../closure-topology.md). The overline on the sum is present in the original PDF and is essential for potentially nonclosed sums.

Take the polar decomposition $T=V|T|$ between these [Hilbert spaces](../../../../../../hilbert-space-split.md). Because $T$ intertwines the two actions of $M$, its adjoint does also, so $T^*T$ commutes with the action on $H_1$. Its positive square root therefore commutes as well. The identity $V|T|\xi=T\xi$ shows on its dense initial range that $V$ intertwines, and [continuity](../../../../../../continuous-function.md) extends this to $K_1$. It is an isometry onto $K_2$. Consequently

$$
\boxed{H_1\cap(H_1\cap H_2)^\perp
\ \cong_M\ \overline{H_1+H_2}\cap H_2^\perp.}
$$

The unitary here is a unitary between the indicated [Hilbert space modules](../../../../../../hilbert-space-module-over-a-von-neumann-algebra.md), not an assertion that the unclosed algebraic sum is a [Hilbert space](../../../../../../hilbert-space-split.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

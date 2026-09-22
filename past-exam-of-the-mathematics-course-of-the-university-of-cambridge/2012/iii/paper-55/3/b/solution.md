<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Work over a coordinate neighborhood $U\subset B$ with coordinates $x^i$, and choose a basis $T_a$ of the [Lie algebra](../../../../../../lie-algebra-split.md), with $[T_a,T_b]=c^c{}_{ab}T_c$. Put $A=A_i^aT_a\,dx^i$. For each $T_a$ let $R_a$ be its [right-invariant vector field](../../../../../../right-invariant-vector-field.md) on the fiber group. In matrix notation $R_a(\gamma)=T_a\gamma$, and

$$
[R_a,R_b]=-c^c{}_{ab}R_c.
$$

This minus sign is the [right-invariant vector fields realize the opposite Lie algebra](../../../../../../right-invariant-vector-fields-realize-the-opposite-lie-algebra.md) rule. It is essential here. Define the [coordinate horizontal lifts of a principal connection](../../../../../../coordinate-horizontal-lifts-of-a-principal-connection.md) by

$$
\boxed{H_i=\partial_i-A_i^aR_a.}
$$

Their projections are $\pi_*H_i=\partial_i$, so they are linearly independent and there are exactly $\dim B$ of them. Also $d\gamma(H_i)=-A_i\gamma$, whence

$$
\omega(H_i)=\gamma^{-1}A_i\gamma+\gamma^{-1}(-A_i\gamma)=0.
$$

They therefore span the [horizontal distribution of a principal connection](../../../../../../horizontal-distribution-of-a-principal-connection.md) on this trivialization.

The coefficients $A_i^a$ depend only on the base variables, so taking [Lie brackets](../../../../../../lie-bracket.md) gives

$$
[H_i,H_j]=-\left(\partial_iA_j^c-\partial_jA_i^c+c^c{}_{ab}A_i^aA_j^b\right)R_c=-F_{ij}^cR_c,
$$

where $F_{ij}=\partial_iA_j-\partial_jA_i+[A_i,A_j]$ and $F=\tfrac12F_{ij}\,dx^i\wedge dx^j=dA+A\wedge A$. Since the [right-invariant vector fields](../../../../../../right-invariant-vector-field.md) form a basis on each fiber, **$\boxed{[H_i,H_j]=0\text{ for all }i,j\iff F=0}$**. This is the local coordinate version of vanishing [curvature of a principal connection](../../../../../../curvature-of-a-principal-connection.md) and, by the [Frobenius theorem](../../../../../../frobenius-theorem.md), integrability of the horizontal distribution.

The coordinate qualification is necessary: horizontal lifts of arbitrary noncommuting base fields need not commute even for a [flat principal connection](../../../../../../flat-principal-connection.md). Nor does flatness guarantee a globally defined coordinate frame or a global horizontal section; [holonomy of a connection](../../../../../../holonomy.md) can obstruct the latter. If the requested frame were read globally, the trivial flat bundle $S^2\times G$ would already be a counterexample: restricting a global horizontal frame to the identity-fiber section would trivialize $TS^2$, contrary to the [Hairy ball theorem](../../../../../../hairy-ball-theorem.md). The construction on each coordinate trivialization supplies the intended result without that global claim.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

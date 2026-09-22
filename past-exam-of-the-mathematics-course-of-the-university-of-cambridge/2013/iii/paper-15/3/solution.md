<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Combining [metric compatibility](../../../../../metric-compatibility.md) with the [torsion-free](../../../../../torsion-free-connection.md) condition forces the [Koszul formula](../../../../../koszul-formula.md):

$$
2g(\nabla_XY,Z)=Xg(Y,Z)+Yg(Z,X)-Zg(X,Y)-g(X,[Y,Z])+g(Y,[Z,X])+g(Z,[X,Y]).
$$

Nondegeneracy of $g$ proves uniqueness of the [Levi-Civita connection](../../../../../levi-civita-connection.md). For existence, use the right side to define $2g(\nabla_XY,Z)$. Expanding brackets shows that this expression is $C^\infty$-linear in $Z$, so it defines a smooth one-form; the [musical isomorphism](../../../../../musical-isomorphism.md) gives the required [vector field](../../../../../vector-field.md). The same expansion shows $\nabla_{aX}Y=a\nabla_XY$, additivity, and $\nabla_X(aY)=X(a)Y+a\nabla_XY$, establishing the connection rules. Subtracting the formulas with $X,Y$ exchanged gives $\nabla_XY-\nabla_YX=[X,Y]$. Adding the formulas pairing $\nabla_XY$ with $Z$ and $\nabla_XZ$ with $Y$ gives [metric compatibility](../../../../../metric-compatibility.md). Thus this construction has both required properties.

In coordinate [vector fields](../../../../../vector-field.md) the brackets vanish. Consequently the [Christoffel symbols](../../../../../christoffel-symbol.md) and coordinate [derivative](../../../../../derivative.md) are

$$
\boxed{\Gamma^k_{ij}=\frac12g^{k\ell}(\partial_i g_{j\ell}+\partial_j g_{i\ell}-\partial_\ell g_{ij}),\qquad
\nabla_XY=\left(X^i\partial_iY^k+\Gamma^k_{ij}X^iY^j\right)\partial_k}.
$$

Repeated indices are summed. The displayed connection type in the source is best understood in its standard form on two [vector fields](../../../../../vector-field.md); if the first input is an individual tangent vector at a point, the output lies in the tangent fiber at that point rather than in the space of global sections.

For the [parallel metrics with a common Levi-Civita connection](../../../../../parallel-metrics-with-a-common-levi-civita-connection.md), let $\gamma$ be a piecewise smooth path from the point $x$ of equality to any $y$. [Connected](../../../../../connected-space.md) [smooth manifolds](../../../../../smooth-manifold.md) admit such paths because coordinate balls are path [connected](../../../../../connected-space.md). [Parallel transport](../../../../../parallel-transport.md) $P_\gamma$ for the common connection is invertible and preserves both metrics. Therefore

$$
\widetilde g_y(P_\gamma u,P_\gamma v)=\widetilde g_x(u,v)=g_x(u,v)=g_y(P_\gamma u,P_\gamma v).
$$

Every pair of tangent vectors at $y$ arises this way, so $\boxed{\widetilde g=g}$ everywhere.

Dropping the agreement at one point removes the conclusion. For any constant $c>0$, $\widetilde g=cg$ has the same [Christoffel symbols](../../../../../christoffel-symbol.md). Nor must the two metrics be proportional: on $\mathbb R^n$, $n\geq2$, the constant metrics $\sum_i(dx^i)^2$ and $2(dx^1)^2+\sum_{i\geq2}(dx^i)^2$ both have zero connection coefficients. In general write $\widetilde g(u,v)=g(Au,v)$. Since both metrics are parallel, $0=(\nabla_X\widetilde g)(Y,Z)=g((\nabla_XA)Y,Z)$, so $\nabla A=0$. Conversely, a positive $g$-self-adjoint parallel $A$ makes the same [torsion-free](../../../../../torsion-free-connection.md) connection compatible with $\widetilde g$, proving equality of their [Levi-Civita connections](../../../../../levi-civita-connection.md). Thus one-point agreement specifies $A=I$ and forces it everywhere; without it, nontrivial parallel choices can remain.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

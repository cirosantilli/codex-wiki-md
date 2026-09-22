<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

At a hyperbolic saddle, the stable invariant subspace of $Df(0)$ is the sum of its [generalized eigenspaces](../../../../../generalized-eigenspace.md) with negative real parts; the unstable subspace uses positive real parts. The [stable manifold theorem](../../../../../stable-manifold-theorem.md) gives invariant local manifolds tangent to these subspaces at the equilibrium, with the corresponding dimensions and the appropriate forward or backward convergence to the equilibrium.

Here the Jacobian is $\operatorname{diag}(1,-1)$, so the unstable tangent is the $x$ axis and the stable tangent the $y$ axis. For the stable graph write $x=h(y)=Ay^2+By^3+O(y^4)$. Invariance requires $h'(y)(-y+3h(y)^2)=h+h^2+2hy+3y^2$. Comparing quadratic and cubic terms gives $-2A=A+3$ and $-3B=B+2A$, so $A=-1,B=1/2$.

For the unstable graph $y=g(x)=Cx^2+Dx^3+O(x^4)$, invariance is $g'(x)(x+x^2+2xg+3g^2)=-g+3x^2$. Coefficients give $2C=3-C$ and $2C+3D=-D$, so $C=1,D=-1/2$. Thus the [cubic graph expansion of a saddle invariant manifold](../../../../../cubic-graph-expansion-of-a-saddle-invariant-manifold.md) is

$$
\boxed{W^s:\ x=-y^2+y^3/2+O(y^4),\qquad W^u:\ y=x^2-x^3/2+O(x^4).}
$$

These describe the local manifolds to cubic order, not exact global [polynomial](../../../../../polynomial-split.md) curves.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

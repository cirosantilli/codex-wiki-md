<h1 id="32b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There are two bifurcations in $0\leq k\leq1/2$, both at $k=0$.

Near $(0,0,0)$, append $\dot k=0$. The plane $y=0$ is invariant and tangent to the extended center subspace, so it is an [extended center manifold](../../../../../../extended-centre-manifold-for-a-parameter.md). The reduced equation is exactly

$$
\dot x=x(-k-3x+x^2),
\qquad
\dot k=0.
$$

Its leading terms $-kx-3x^2$ have two branches, $x=0$ and $x=-k/3+O(k^2)$, which cross and exchange their center-direction stability. Hence this is a [transcritical bifurcation](../../../../../../transcritical-bifurcation.md).

For the bifurcation at $(1,2,0)$, set

$$
X=x-1,\qquad v=y-2-X.
$$

The extended system becomes

$$
\dot X=(1+X)(v-k+X^2),
\qquad
\dot v=v+v^2+(1+X)(k-X^2),
\qquad
\dot k=0.
$$

Solving the [centre-manifold invariance equation](../../../../../../centre-manifold-invariance-equation.md) for $v=h(X,k)$ gives

$$
h(X,k)=-k+X^2-5Xk+9k^2+O\bigl((|X|+|k|)^3\bigr).
$$

Substitution into the $X$ equation yields

$$
\dot X=2(X^2-k)+O\bigl((|X|+|k|)^3\bigr).
$$

For $k>0$ this has two nearby equilibria $X=\pm\sqrt k+O(k)$, while for $k<0$ it has none. It is therefore a [saddle-node bifurcation](../../../../../../saddle-node-bifurcation.md). These reductions are collected in [bifurcations of the 2022 Cambridge quadratic-cubic system](../../../../../../bifurcations-of-the-2022-cambridge-quadratic-cubic-system.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [32B](../../32b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

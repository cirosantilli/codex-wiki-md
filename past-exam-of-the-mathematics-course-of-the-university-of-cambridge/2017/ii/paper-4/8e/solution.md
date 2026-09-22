<h1 id="8e/solution">Solution</h1>

↑ **Parent:** [8E](../8e.md)

The [Poisson bracket](../../../../../poisson-bracket.md) is $\{f,g\}=\mathbf r\cdot(\nabla f\times\nabla g)$. Since $\nabla\rho^2=2\mathbf r$, the [scalar triple product](../../../../../scalar-triple-product.md) vanishes, and

$$
\boxed{\{f,\rho^2\}=0.}
$$

Equivalently, check the identity on $x,y,z$ and extend to every [polynomial](../../../../../polynomial-split.md) using the [Leibniz rule](../../../../../leibniz-rule.md). Thus $\rho^2$ is a [Casimir function of a Poisson manifold](../../../../../casimir-function-of-a-poisson-manifold.md) of this [rotational Lie-Poisson structure on R3](../../../../../rotational-lie-poisson-structure-on-r3.md).

The [Hamilton's equations](../../../../../hamilton-s-equations.md) are

$$
\boxed{\dot x=(B-C)yz,\qquad\dot y=(C-A)xz,\qquad\dot z=(A-B)xy.}
$$

[Linearization](../../../../../linearization.md) about $(1,0,0)$ gives $\dot\alpha=0$, $\dot\beta=(C-A)\gamma$, $\dot\gamma=(A-B)\beta$. The two nonzero exponents satisfy $\lambda^2=(C-A)(A-B)$. Consequently

$$
\boxed{\text{exponential instability occurs iff }\min(B,C)<A<\max(B,C).}
$$

When $A$ is outside this interval the transverse motion is oscillatory. At equality the [linearization](../../../../../linearization.md) is nonhyperbolic; if just one transverse coupling vanishes, the other permits secular linear growth, rather than an exponential instability. This is the familiar intermediate-axis instability described by the [Euler equations for a torque-free rigid body](../../../../../euler-equations-for-a-torque-free-rigid-body.md).

## ↑ Ancestors (10)

1. [8E](../8e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Multiply [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) by the [displacement](../../../../displacement.md) and integrate. [Integration by parts](../../../../integration-by-parts.md) and the [traction](../../../../traction.md) condition give

$$
0=\int_B\mathbf u\cdot(\nabla\cdot T+\rho\mathbf g)\,dV
=\int_{\partial B}\mathbf u\cdot\boldsymbol\sigma\,dS-\int_BT:\nabla\mathbf u\,dV+\int_B\rho\mathbf u\cdot\mathbf g\,dV.
$$

The [stress](../../../../stress.md) is symmetric, so it contracts only with the symmetric part of $\nabla\mathbf u$, namely $e$. [Hooke's law](../../../../hooke-s-law.md) then gives $T:e=\lambda(\operatorname{tr}e)^2+2\mu e:e=2W$. Hence

$$
\boxed{\int_B\rho\mathbf u\cdot\mathbf g\,dV=\int_B2W\,dV-\int_{\partial B}\mathbf u\cdot\boldsymbol\sigma\,dS.}
$$

The identity is the linear-elastic work balance: twice the stored quadratic energy equals the body-force and boundary-[traction](../../../../traction.md) work paired with the final [displacement](../../../../displacement.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the elasticity and plasticity course of the University of Oxford](../../../split.md)
5. [Elasticity and plasticity course of the University of Oxford](../../../../elasticity-and-plasticity-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

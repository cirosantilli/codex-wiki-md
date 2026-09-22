<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

A form of the [Poincaré-Bendixson theorem](../../../../../poincare-bendixson-theorem.md) states that a nonempty [omega-limit set](../../../../../omega-limit-set.md) of a forward orbit of a $C^1$ planar autonomous [vector](../../../../../vector.md) field, contained in a compact region and containing no [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md), is a [periodic orbit](../../../../../periodic-orbit.md).

Set $\rho=x^2+y^2$. Direct calculation gives

$$
\dot\rho=2\rho(1-\rho)-4k^2x^2y^2,
\qquad2\rho-(2+k^2)\rho^2\leq\dot\rho\leq2\rho(1-\rho),
$$

because $0\leq x^2y^2\leq\rho^2/4$. At the inner boundary $\rho=2/(2+k^2)$ the flow points into or along the annulus, and at the outer boundary $\rho=1$ it does likewise. Smoothness and these inequalities make the compact annulus forward invariant.

For nonzero $(x,y)$, write $x=\sqrt\rho\cos\theta$, $y=\sqrt\rho\sin\theta$. Then

$$
\dot\theta=\frac{x\dot y-y\dot x}{\rho}
=1-\frac{k^2\rho}{4}\sin4\theta\geq1-\frac{k^2}{4}>0
$$

throughout the annulus. Hence it contains no [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md). Any orbit starting there remains compactly trapped, has a nonempty [omega-limit set](../../../../../omega-limit-set.md), and the [Poincaré-Bendixson theorem](../../../../../poincare-bendixson-theorem.md) supplies the required **[periodic orbit](../../../../../periodic-orbit.md) in the stated annulus**. For $k=0$ the annulus reduces to $\rho=1$ itself, and there $\dot\theta=1$, giving the [periodic orbit](../../../../../periodic-orbit.md) directly.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

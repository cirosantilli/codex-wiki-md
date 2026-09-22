<h1 id="1c/solution">Solution</h1>

↑ **Parent:** [1C](../1c.md)

This is a [logistic equation](../../../../../logistic-differential-equation.md), with positive [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md) $N=\alpha$ and initial population above that value. On the positive branch, put $v=1/N$. It satisfies the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md) $v'+\alpha v=1$, so $v=\alpha^{-1}+Ce^{-\alpha t}$. The initial condition gives $C=-1/(2\alpha)$, hence

$$
\boxed{N(t)=\frac{\alpha}{1-\tfrac12e^{-\alpha t}}
=\frac{2\alpha}{2-e^{-\alpha t}},\qquad \lim_{t\to\infty}N(t)=\alpha.}
$$

The population decreases monotonically toward the stable [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md); it never reaches it at a finite time.

## ↑ Ancestors (10)

1. [1C](../1c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

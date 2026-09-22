<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

Assume the velocity-to-momentum Legendre map is locally invertible. Differentiate the [Hamiltonian](../../../../../hamiltonian.md) while regarding $q,p,t$ as independent:

$$
dH=\sum_i\dot q_i\,dp_i+\sum_i p_i\,d\dot q_i-dL=\sum_i\dot q_i\,dp_i-\sum_i\frac{\partial L}{\partial q_i}dq_i-\frac{\partial L}{\partial t}dt.
$$

The velocity variations cancel because $p_i=\partial L/\partial\dot q_i$. Combining the remaining coefficients with the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) gives [Hamilton's equations](../../../../../hamilton-s-equations.md)

$$
\boxed{\dot q_i=\frac{\partial H}{\partial p_i},\qquad\dot p_i=-\frac{\partial H}{\partial q_i}.}
$$

An [ignorable coordinate](../../../../../ignorable-coordinate.md) does not occur explicitly in the Lagrangian, so its conjugate momentum is conserved. For the spherical motion, $\phi$ is ignorable and the [Hamiltonian](../../../../../hamiltonian.md) has no explicit time dependence. The two constants are **$p_\phi$ and $H$**.

The polar [Hamilton equations](../../../../../hamilton-s-equations.md) are

$$
\dot\theta=\frac{p_\theta}{ma^2},\qquad\dot p_\theta=\frac{p_\phi^2\cos\theta}{ma^2\sin^3\theta}-V'(\theta).
$$

A constant polar angle therefore requires $p_\theta=0$ and vanishing of the second right-hand side. For $0<\theta<\pi$ with $\cos\theta\ne0$, this is

$$
\boxed{p_\phi^2=\frac{ma^2\sin^3\theta}{\cos\theta}V'(\theta).}
$$

The expression must be nonnegative to represent a real momentum. Once it holds, $\phi$ advances uniformly at $p_\phi/(ma^2\sin^2\theta)$, so it is also sufficient with those initial data. At the equator the undivided equation instead requires $V'(\pi/2)=0$, with any $p_\phi$; dividing by cosine would wrongly discard this special case. The polar coordinate chart itself excludes the poles.

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

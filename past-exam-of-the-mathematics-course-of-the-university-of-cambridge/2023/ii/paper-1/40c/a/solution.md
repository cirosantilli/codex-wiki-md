<h1 id="40c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\rho'$ and $p'$ be the density and pressure perturbations and let $\mathbf u$ be the velocity perturbation. The [linear acoustics](../../../../../../linear-acoustics-split.md) equations about a uniform quiescent state are

$$
\rho'_t+\rho_0\nabla\mathbin{\cdot}\mathbf u=0,
\qquad
\rho_0\mathbf u_t=-\nabla p',
\qquad
p'=c_0^2\rho'.
$$

The last relation is the [homentropic pressure perturbation](../../../../../../homentropic-pressure-perturbation.md) law.

Taking the scalar product of the momentum equation with $\mathbf u$ gives

$$
\frac{\partial}{\partial t}\left(\frac12\rho_0|\mathbf u|^2\right)
=-\mathbf u\mathbin{\cdot}\nabla p'
=-\nabla\mathbin{\cdot}(p'\mathbf u)+p'\nabla\mathbin{\cdot}\mathbf u.
$$

The continuity and pressure relations imply

$$
p'\nabla\mathbin{\cdot}\mathbf u
=-\frac{p'p'_t}{\rho_0c_0^2}
=-\frac\partial{\partial t}
\left(\frac{p'^2}{2\rho_0c_0^2}\right).
$$

Therefore the [acoustic energy conservation](../../../../../../acoustic-energy-conservation.md) law is

$$
\boxed{
\frac\partial{\partial t}(K+W)+\nabla\mathbin{\cdot}\mathbf I=0
},
$$

with

$$
\boxed{
K=\frac12\rho_0|\mathbf u|^2,
\qquad
W=\frac{p'^2}{2\rho_0c_0^2},
\qquad
\mathbf I=p'\mathbf u
}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [40C](../../40c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

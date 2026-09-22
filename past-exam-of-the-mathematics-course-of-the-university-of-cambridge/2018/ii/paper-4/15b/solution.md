<h1 id="15b/solution">Solution</h1>

↑ **Parent:** [15B](../15b.md)

Define the [canonical momenta](../../../../../canonical-momentum.md)

$$
p_i=\frac{\partial\mathcal L}{\partial\dot q_i}.
$$

When the velocity Hessian is nonsingular, these equations can be inverted for $\dot q_i(q,p,t)$, and the [Hamiltonian](../../../../../hamiltonian.md) is the [Legendre transform](../../../../../convex-conjugate.md)

$$
\boxed{H(q,p,t)=\sum_i p_i\dot q_i-\mathcal L(q,\dot q,t).}
$$

Its differential is

$$
dH=\sum_i\dot q_i\,dp_i
-\sum_i\frac{\partial\mathcal L}{\partial q_i}\,dq_i
-\frac{\partial\mathcal L}{\partial t}\,dt,
$$

because the $p_i\,d\dot q_i$ terms cancel. The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) identifies $\partial\mathcal L/\partial q_i=\dot p_i$, so coefficient comparison gives [Hamilton's equations](../../../../../hamilton-s-equations.md)

$$
\boxed{\dot q_i=\frac{\partial H}{\partial p_i},
\qquad
\dot p_i=-\frac{\partial H}{\partial q_i}.}
$$

For the [symmetric top](../../../../../symmetric-top.md), the momenta are

$$
p_\theta=A\dot\theta,
\qquad
p_\psi=B(\dot\psi+\dot\phi\cos\theta),
\qquad
p_\phi=A\dot\phi\sin^2\theta+p_\psi\cos\theta.
$$

Thus

$$
\dot\theta=\frac{p_\theta}{A},
\qquad
\dot\phi=\frac{p_\phi-p_\psi\cos\theta}{A\sin^2\theta},
\qquad
\dot\psi=\frac{p_\psi}{B}-\dot\phi\cos\theta.
$$

The Legendre transform gives

$$
\boxed{H=
\frac{p_\theta^2}{2A}
+\frac{(p_\phi-p_\psi\cos\theta)^2}{2A\sin^2\theta}
+\frac{p_\psi^2}{2B}
+Mgl\cos\theta.}
$$

Both $\phi$ and $\psi$ are [cyclic coordinates](../../../../../cyclic-coordinate.md), so $p_\phi$ and $p_\psi$ are conserved. The Hamiltonian has no explicit time dependence and is also conserved. Since $H$ is independent of $\phi,\psi$,

$$
\{H,p_\phi\}=\{H,p_\psi\}=\{p_\phi,p_\psi\}=0
$$

under the [Poisson bracket](../../../../../poisson-bracket.md). Hence three independent [first integrals in involution](../../../../../first-integrals-in-involution.md) are

$$
\boxed{H,\qquad p_\phi,\qquad p_\psi.}
$$

## ↑ Ancestors (10)

1. [15B](../15b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

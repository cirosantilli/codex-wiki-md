<h1 id="9d/solution">Solution</h1>

↑ **Parent:** [9D](../9d.md)

In [Lagrangian mechanics](../../../../../lagrangian-mechanics.md), the [energy balance for an autonomous Lagrangian](../../../../../energy-balance-for-an-autonomous-lagrangian.md) uses $E=\sum_i\dot q_i\,\partial L/\partial\dot q_i-L$. For the stationary [vector potential](../../../../../vector-potential.md) the velocity-linear magnetic term cancels in this expression, leaving [kinetic energy](../../../../../kinetic-energy.md). In [cylindrical coordinates](../../../../../cylindrical-coordinate-system.md),

$$
L=\frac m2(\dot r^2+r^2\dot\phi^2+\dot z^2)+er^2g(z)\dot\phi.
$$

Time independence and the cyclic angular coordinate give two constants:

$$
\boxed{E=\frac m2(\dot r^2+r^2\dot\phi^2+\dot z^2),\qquad
p_\phi=mr^2\dot\phi+er^2g(z).}
$$

The three [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are

$$
m\ddot r=mr\dot\phi^2+2erg\dot\phi,\qquad
\frac d{dt}(mr^2\dot\phi+er^2g)=0,\qquad
m\ddot z=er^2g'\dot\phi.
$$

The supplied angular velocity is $\dot\phi=-2eg(z_0)/m$. Set $r=r_0$, $z=z_0$ and use this constant angular velocity. The radial right-hand side is $mr_0(\dot\phi^2+2eg\dot\phi/m)=0$, the [angular momentum](../../../../../angular-momentum.md) is constant, and the vertical equation vanishes when $g'(z_0)=0$. These equations and the initial data therefore give

$$
\boxed{r(t)=r_0,\quad z(t)=z_0,\quad
\phi(t)=\phi_0-\frac{2eg(z_0)}m t.}
$$

For nonzero radius and charge this is the requested circular orbit.

## ↑ Ancestors (10)

1. [9D](../9d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

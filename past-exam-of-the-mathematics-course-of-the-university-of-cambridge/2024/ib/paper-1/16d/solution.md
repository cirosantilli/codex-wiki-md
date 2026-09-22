<h1 id="16d/solution">Solution</h1>

↑ **Parent:** [16D](../16d.md)

Let $x$ point downslope and $z$ point normally away from the plane, with $0\leq z\leq h$. Write the parallel [velocity](../../../../../velocity.md) as $u(z)e_x$ and take $\tau>0$ to be the magnitude of the air's upslope stress. The steady equations are

$$
0=-p_x+\rho g\sin\alpha+\mu u'',
\qquad
0=-p_z-\rho g\cos\alpha,
$$

with [boundary conditions](../../../../../boundary-condition.md)

$$
u(0)=0,
\qquad
p(h)=p_0,
\qquad
\mu u'(h)=-\tau.
$$

The free-surface condition makes $p_x=0$, and integration gives

$$
\boxed{p(x,z)=p_0+\rho g\cos\alpha\,(h-z)},
$$



$$
\boxed{u(z)=\frac{\rho g\sin\alpha}{\mu}
\left(hz-\frac{z^2}{2}\right)-\frac{\tau z}{\mu}}.
$$

The surface [velocity](../../../../../velocity.md), downslope shear exerted by the fluid on the plane, and volume flux per unit width are

$$
\boxed{u_h=\frac h\mu\left(\frac{\rho gh\sin\alpha}{2}-\tau\right)},
$$



$$
\boxed{\tau_0=\mu u'(0)=\rho gh\sin\alpha-\tau},
$$



$$
\boxed{q=\int_0^hu(z)\,dz
=\frac{\rho g h^3\sin\alpha}{3\mu}
-\frac{\tau h^2}{2\mu}}.
$$

Thus the [inclined viscous film with opposing surface shear](../../../../../inclined-viscous-film-with-opposing-surface-shear.md) reverses in the three senses when

$$
\begin{array}{c|c}
\text{quantity directed upslope}&\text{condition}\\ \hline
u_h&\tau>\frac12\rho gh\sin\alpha\\
q&\tau>\frac23\rho gh\sin\alpha\\
\tau_0&\tau>\rho gh\sin\alpha.
\end{array}
$$

The order of increasing required air stress is therefore

$$
\boxed{\text{surface velocity},\quad\text{volume flux},\quad\text{stress on the plane}}.
$$

## ↑ Ancestors (10)

1. [16D](../16d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

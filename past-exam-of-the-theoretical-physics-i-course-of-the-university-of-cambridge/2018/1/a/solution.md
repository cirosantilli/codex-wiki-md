<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Choose [Minkowski metric](../../../../minkowski-metric.md) $(+,-,-,-)$, so $A_\mu=(\phi/c,-\mathbf A)$ and $d\tau=dt\sqrt{1-v^2/c^2}$. In laboratory time the [relativistic charged-particle action](../../../../relativistic-charged-particle-action.md) has [Lagrangian](../../../../lagrangian.md)

$$
L=-mc^2\sqrt{1-v^2/c^2}-e\phi(\mathbf x,t)+e\mathbf A(\mathbf x,t)\cdot\mathbf v.
$$

Here $e$ denotes the signed particle charge in the action. The [canonical momentum](../../../../canonical-momentum.md) and the position derivative are

$$
\frac{\partial L}{\partial v_i}=m\gamma v_i+eA_i,\qquad
\frac{\partial L}{\partial x_i}=-e\partial_i\phi+e v_j\partial_iA_j,
\qquad \gamma=(1-v^2/c^2)^{-1/2}.
$$

The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) therefore gives

$$
\frac d{dt}(m\gamma v_i)=e\left[-\partial_i\phi-\partial_t A_i+v_j(\partial_iA_j-\partial_jA_i)\right].
$$

The last term is $(\mathbf v\times\mathbf B)_i$, and the first two terms form the [electric field](../../../../electric-field-split.md). Thus the [relativistic Lorentz force](../../../../relativistic-lorentz-force.md) equation is

$$
\boxed{\frac d{dt}(m\gamma\mathbf v)=e(\mathbf E+\mathbf v\times\mathbf B).}
$$

Its power relation and acceleration form are

$$
\boxed{\frac d{dt}(\gamma mc^2)=e\mathbf E\cdot\mathbf v,\qquad
\dot{\mathbf v}=\frac e{m\gamma}\left[\mathbf E+\mathbf v\times\mathbf B-\frac{\mathbf v(\mathbf E\cdot\mathbf v)}{c^2}\right].}
$$

The power relation follows by taking the scalar product with $\mathbf v$ and using the [relativistic energy-momentum relation](../../../../energy-momentum-relation.md). It also shows why the [magnetic field](../../../../magnetic-field-split.md) alone cannot change the particle's energy.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)

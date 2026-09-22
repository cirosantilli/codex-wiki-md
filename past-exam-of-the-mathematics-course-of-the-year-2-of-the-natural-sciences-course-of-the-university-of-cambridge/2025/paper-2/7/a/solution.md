<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathbf q=(x,y)$ be the centre displacement and $\theta$ the small disk rotation. Put $d=l-l_0>0$. The [moment of inertia of a uniform disc](../../../../../moment-of-inertia-of-a-uniform-disc.md) is $I=ma^2/2$, obtained from $I=\int_0^a\rho r^2(2\pi r\,dr)$ and $m=\rho\pi a^2$. Thus the [kinetic energy](../../../../../kinetic-energy.md) is $T=m|\dot{\mathbf q}|^2/2+ma^2\dot\theta^2/4$.

For one spring, let $\mathbf n_j$ point radially towards its fixed anchor and let $\mathbf t_j$ be the perpendicular unit [vector](../../../../../vector.md). The moving attachment is $\mathbf q+aR(\theta)\mathbf n_j$, while the anchor is $(a+l)\mathbf n_j$. Expanding their separation to second order gives the spring extension beyond natural length:

$$
s_j-l_0=d-\mathbf n_j\cdot\mathbf q+\frac a2\theta^2+
\frac{(\mathbf t_j\cdot\mathbf q+a\theta)^2}{2l}+O((|\mathbf q|+|\theta|)^3).
$$

Insert this in the [elastic potential energy](../../../../../elastic-energy.md) $V=(k/2)\sum_j(s_j-l_0)^2$. For the three symmetric directions, $\sum_j\mathbf n_j=\sum_j\mathbf t_j=0$ and $\sum_j(\mathbf n_j\cdot\mathbf q)^2=\sum_j(\mathbf t_j\cdot\mathbf q)^2=3|\mathbf q|^2/2$. Dropping the constant equilibrium energy gives

$$
V_2=\frac{3k}{4}\left(1+\frac dl\right)(x^2+y^2)+\frac{3kda(a+l)}{2l}\theta^2.
$$

Therefore the quadratic [Lagrangian](../../../../../lagrangian.md) is

$$
\boxed{\mathcal L_2=\frac m2(\dot x^2+\dot y^2)+\frac{ma^2}4\dot\theta^2-\frac{3k}{4}\left(1+\frac dl\right)(x^2+y^2)-\frac{3kda(a+l)}{2l}\theta^2.}
$$

The prestretch terms cannot be omitted: they supply transverse spring stiffness and the entire rotational restoring torque, as derived generally in [small oscillations of a disk attached to prestretched radial springs](../../../../../small-oscillations-of-a-disk-attached-to-prestretched-radial-springs.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

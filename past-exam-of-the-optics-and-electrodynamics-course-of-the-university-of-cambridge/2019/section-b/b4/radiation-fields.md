<h1 id="section-b/b4/radiation-fields">Radiation fields</h1>

↑ **Parent:** [Solution](solution.md)

The consistent [Liénard–Wiechert potential](../../../../lienard-wiechert-potential.md) obeys $\mathbf A=\mathbf u\varphi/c^2$. To first order in $\boldsymbol\beta=\mathbf u/c$, its large-distance form is

$$
\varphi\simeq\frac{q}{4\pi\epsilon_0r}[1+\mathbf n\cdot\boldsymbol\beta(t_r)],\qquad
\mathbf A\simeq\frac{\mu_0q}{4\pi r}\mathbf u(t_r),\qquad
t_r\simeq t-\frac rc.
$$

Terms varying as $1/r^2$ give near fields and are negligible for the radiated [power](../../../../power.md) at large $r$. Keep the first-order velocity term in $\varphi$: although small, its retarded-time derivative contributes a leading [acceleration](../../../../acceleration.md) field. To the required order, $\partial t_r/\partial t\simeq1$ and $\nabla t_r\simeq-\mathbf n/c$. Holding the observation direction fixed at leading order gives

$$
-\nabla\varphi\big|_{1/r}=\frac{q}{4\pi\epsilon_0cr}\mathbf n(\mathbf n\cdot\dot{\boldsymbol\beta}),\qquad
-\frac{\partial\mathbf A}{\partial t}\bigg|_{1/r}=-\frac{q}{4\pi\epsilon_0cr}\dot{\boldsymbol\beta}.
$$

Thus the outgoing [electric field](../../../../electric-field-split.md) is transverse:

$$
\boxed{\mathbf E_{\rm rad}(\mathbf r,t)=\frac{q}{4\pi\epsilon_0c r}
\left[\mathbf n\times(\mathbf n\times\dot{\boldsymbol\beta})\right]_{t_r}
=\frac{q}{4\pi\epsilon_0c^2r}
\left[\mathbf n\times(\mathbf n\times\mathbf a)\right]_{t_r}.}
$$

Here $\mathbf a=d\mathbf u/dt_r$. The [magnetic field](../../../../magnetic-field-split.md) follows from $\nabla\times\mathbf A$, or from the outgoing [plane electromagnetic wave](../../../../plane-electromagnetic-wave.md) relation:

$$
\boxed{\mathbf B_{\rm rad}=-\frac{\mu_0q}{4\pi r}
[\mathbf n\times\dot{\boldsymbol\beta}]_{t_r}
=\frac1c\mathbf n\times\mathbf E_{\rm rad}.}
$$

The minus sign is essential. Both fields fall as $1/r$, are mutually orthogonal and obey $|\mathbf E|=c|\mathbf B|$. The corresponding [Liénard-Wiechert field](../../../../lienard-wiechert-field.md) also contains nonradiative terms, omitted in this leading far-field calculation.

## ↑ Ancestors (14)

1. [Solution](solution.md)
2. [B4](../b4.md)
3. [Section B](../../section-b.md)
4. [2019](../../../2019-split.md)
5. [Past exam of the optics and electrodynamics course of the University of Cambridge](../../../split.md)
6. [Optics and Electrodynamics course of the University of Cambridge](../../../../optics-and-electrodynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)

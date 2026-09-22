<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

Insert $\nabla\times\mathbf E=-\partial_t\mathbf B$ and $\nabla\times\mathbf H=\mathbf J+\partial_t\mathbf D$ into the given identity. For a linear, time-independent, nondispersive medium, $\mathbf D=\epsilon\mathbf E$ and $\mathbf B=\mu\mathbf H$, giving

$$
\nabla\cdot(\mathbf E\times\mathbf H)=-\mathbf J\cdot\mathbf E-\partial_tu,
\qquad u=\frac12\mathbf E\cdot\mathbf D+\frac12\mathbf H\cdot\mathbf B.
$$

The [divergence theorem](../../../../../divergence-theorem.md) then yields

$$
\boxed{\oint_S(\mathbf E\times\mathbf H)\cdot d\mathbf S=-\int_V[\mathbf J\cdot\mathbf E+\partial_tu]\,dV.}
$$

The left side is outward electromagnetic [power](../../../../../power.md) flow. The current term is [power](../../../../../power.md) delivered to matter, becoming [Joule heating](../../../../../joule-heating.md) for an [Ohmic conductor](../../../../../ohmic-conductor.md), and $\partial_tu$ is the change in stored electric plus [magnetic energy](../../../../../magnetic-energy.md). The minus sign says outward flux reduces stored [energy](../../../../../energy-split.md) unless supplied locally.

Follow the drawing's coordinates: lower strip at $z=0$, upper strip at $z=d$, current $I$ along $+x$ in the upper strip and back along the lower. The wording “both strips lie in the $xy$-plane” must mean parallel to that plane, since the drawing separates them in $z$. Neglect the side and end fringes using $l\gg a\gg d$. Then $I=V_0/(R+R_L)$ and the top-strip potential is $V(x)=V_0-IRx/l$, while the lower strip is equipotential at zero.

The harmonic function matching those two surfaces is

$$
\boxed{\phi=\frac zd\left(V_0-\frac{IRx}{l}\right).}
$$

Indeed $\nabla^2\phi=0$, and it has the required potentials at $z=0,d$. Thus

$$
\mathbf E=\left(\frac{IRz}{ld},0,-\frac{V(x)}d\right),\qquad
\mathbf H=\left(0,\frac Ia,0\right).
$$

The two current sheets reinforce their [magnetic field](../../../../../magnetic-field-split.md) between the strips; its direction follows the right-hand rule. The [Poynting flow in resistive parallel strips](../../../../../poynting-flow-in-resistive-parallel-strips.md) follows from their cross product:

$$
\boxed{\mathbf S=\left(\frac{IV(x)}{ad},\ 0,\ \frac{I^2Rz}{ald}\right).}
$$

[Power](../../../../../power.md) flows along the gap towards the load and upwards into the resistive strip. Across a transverse area $ad$, $P_x(x)=IV(x)$ falls from $IV_0$ to $I^2R_L$. The upper surface receives $\int_0^l aS_z(z=d)\,dx=I^2R$, exactly the strip's heating; the ideal lower strip receives none. In the charge-free gap, $\partial_xS_x+\partial_zS_z=0$, consistent with a static field and no local dissipation. The small longitudinal [electric field](../../../../../electric-field-split.md) cannot be discarded if this upward [energy](../../../../../energy-split.md) transfer is to be represented.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

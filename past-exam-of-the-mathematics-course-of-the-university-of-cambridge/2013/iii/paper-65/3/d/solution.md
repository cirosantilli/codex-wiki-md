<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the shallow, equal-density approximation, melting supplies water at rate $v_m$ per unit wetted area. Combining this source with the pressure-driven [volume flux](../../../../../../volumetric-flow-rate.md) gives the [melting-source gravity-current equation](../../../../../../melting-source-gravity-current-equation.md),

$$
\boxed{h_t+q_x=v_m,\qquad q=-Dh^2h_x,\qquad
h_t=D(h^2h_x)_x+v_m}
$$

inside the wet region, with no melting source ahead of the front. In the PDF's signed convention this is $h_t+\gamma(h^2h_x)_x=v_m$. If ice and water densities are distinguished, the meltwater-volume source is $s_m=(\rho_i/\rho_w)v_m$; the same equations then use $s_m$. Geometrical excavation of ice has rate $v_m$, so a density difference requires the confining ice/water-volume mechanics to be treated consistently. The equal-density shallow model identifies these two volumes.

Let $x_-(t)<x_+(t)$ bound the current, and $\mathcal A(t)=\int_{x_-}^{x_+}h\,dx$ be its volume per span. The moving-boundary integral of continuity is

$$
\boxed{\dot{\mathcal A}=s_m(x_+-x_-)-q(x_+)+q(x_-)
+h(x_+)\dot x_+-h(x_-)\dot x_-.}
$$

This exhibits both the melting contribution and any volume swept out by an advancing boundary. For a dry zero-height nose at each end, with no flux through those ends, the boundary terms vanish and

$$
\boxed{\dot{\mathcal A}=s_m\mathcal L(t),\qquad
\ddot{\mathcal A}=s_m\dot{\mathcal L}(t),\qquad \mathcal L=x_+-x_-,}
$$

where the second relation uses constant $s_m$. For a symmetric pulse $\mathcal L=2L$, these become $\dot{\mathcal A}=2s_mL$ and $\ddot{\mathcal A}=2s_m\dot L$; on a reflecting half-line they are $s_mL$ and $s_m\dot L$. Multiplication by $B_y$ gives the three-dimensional water volume.

The [meltwater production over an advancing footprint](../../../../../../meltwater-production-over-an-advancing-footprint.md) can equivalently be expressed as $\mathcal A_m(t)=s_m\int_0^t\mathcal L(t')\,dt'$. At an individual position melting begins only at its wetting time, so new area contributes no finite melt thickness at the instant of arrival. Advancement enlarges the area subsequently melting and hence increases the volume-production rate. The fixed-volume similarity from part (b) cannot simply be reused after adding this source.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

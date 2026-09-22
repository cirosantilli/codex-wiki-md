<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**Correction of the printed limits:** ordinary positive [polymer contour length](../../../../polymer-contour-length.md) requires integration from $R_{\rm in}$ to $R_{\rm out}$, because $R_{\rm out}>R_{\rm in}$ and the ring count is positive. For example, taking $n(R)=1$, $R_{\rm out}=2$ and $R_{\rm in}=1$ makes the printed outward-to-inward integral negative. Thus its sign cannot be retained as a physical length.

For hexagonally packed strands choose axial ring spacing $s$ and radial layer spacing $\sqrt3s/2$. With $n=h/s$ and radial layer density $2/(\sqrt3s)$,

$$
L=\frac{2}{\sqrt3s}\int_{R_{\rm in}}^{R_{\rm out}}2\pi R\frac hs\,dR
=\frac{2\pi h}{\sqrt3s^2}(R_{\rm out}^2-R_{\rm in}^2).
$$

The same continuum replacement in [b](../b.md) gives

$$
\Delta G_{\rm elastic}
=\frac{2\pi l_pk_BT h}{\sqrt3s^2}\ln\frac{R_{\rm out}}{R_{\rm in}},\qquad
R_{\rm in}^2=R_{\rm out}^2-\frac{\sqrt3s^2L}{2\pi h}.
$$

Eliminating the inner radius yields

$$
\boxed{\Delta G_{\rm elastic}
=\frac{\pi l_pk_BT h}{\sqrt3s^2}
\ln\left(\frac{R_{\rm out}^2}{R_{\rm out}^2-\sqrt3s^2L/(2\pi h)}\right).}
$$

The resisting packaging [force](../../../../force-split.md) is the marginal [free energy](../../../../thermodynamic-free-energy.md) per added [polymer contour length](../../../../polymer-contour-length.md), at fixed $h$, $s$ and $R_{\rm out}$:

$$
\boxed{F_L=\left(\frac{\partial\Delta G_{\rm elastic}}{\partial L}\right)_{h,s,R_{\rm out}}
=\frac{l_pk_BT}{2R_{\rm in}^2}
=\frac{l_pk_BT}{2\left(R_{\rm out}^2-\sqrt3s^2L/(2\pi h)\right)}.}
$$

The [force](../../../../force-split.md) opposing insertion is positive; its contribution to outward ejection has the same magnitude. The domain is $0\leq L<2\pi hR_{\rm out}^2/(\sqrt3s^2)$. The divergence as the inner hole closes reflects the singular curvature of ideal rings and marks breakdown of the continuum model. If spacing also relaxes, the full [free energy](../../../../thermodynamic-free-energy.md) must include interstrand interactions before optimization; simply varying $s$ in this bending-only formula is insufficient.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

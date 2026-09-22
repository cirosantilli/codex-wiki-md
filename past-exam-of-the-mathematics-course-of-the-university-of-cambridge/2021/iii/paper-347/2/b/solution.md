<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Well inside the [Bondi accretion](../../../../../../bondi-accretion.md) radius, pressure is negligible and the inflow approaches the [free-fall speed](../../../../../../free-fall-speed.md)

$$
v(r)=\sqrt{\frac{2GM_{\rm BH}}r}
=c\sqrt{\frac{r_S}r},
\qquad r_S=\frac{2GM_{\rm BH}}{c^2}.
$$

Steady spherical [mass conservation](../../../../../../mass-conservation.md) gives

$$
\rho=\frac{\dot M}{4\pi r^2v}.
$$

Estimating the outward [optical depth](../../../../../../optical-depth.md) across a radial scale $r$ with electron-scattering opacity $\kappa=\sigma_T/m_p$,

$$
\boxed{\tau(r)\simeq\kappa\rho r
=\frac{\kappa\dot M}{4\pi\sqrt{2GM_{\rm BH}r}}}.
$$

The integral optical depth to infinity differs only by a factor of two in this free-fall approximation.

At the [Schwarzschild radius](../../../../../../schwarzschild-radius.md), $\tau=1$ when

$$
\boxed{\dot M_{\rm crit}
=\frac{8\pi GM_{\rm BH}}{\kappa c}
=\frac{2L_{\rm Edd}}{c^2}}.
$$

If the conventional [Eddington accretion rate](../../../../../../eddington-accretion-rate.md) is $\dot M_{\rm Edd}=L_{\rm Edd}/(\eta_0c^2)$, then $\dot M_{\rm crit}=2\eta_0\dot M_{\rm Edd}$. This comparison depends on the reference efficiency $\eta_0$, while $\dot M_{\rm crit}$ itself follows directly from optical depth.

Writing $\dot m=\dot M/\dot M_{\rm crit}$ gives

$$
\tau(r)=\dot m\sqrt{\frac{r_S}r}.
$$

For $\dot m>1$, the inner flow is optically thick and its [photosphere](../../../../../../photosphere.md) lies at

$$
\boxed{r_{\rm ph}=\dot m^2r_S}.
$$

The diffusion speed is $v_{\rm diff}\sim c/\tau$. Hence

$$
\frac{v}{v_{\rm diff}}
=\frac{v\tau}{c}=\dot m\frac{r_S}r,
$$

and equality defines the [photon-trapping radius](../../../../../../photon-trapping-radius.md)

$$
\boxed{r_t=\dot m\,r_S}.
$$

Inside $r_t$, inward advection outruns outward diffusion, so [photon trapping in an accretion flow](../../../../../../photon-trapping-in-an-accretion-flow.md) carries most released radiation into the black hole.

Only the binding energy released outside $r_t$ escapes efficiently. Its order of magnitude is

$$
L\simeq\frac{GM_{\rm BH}\dot M}{r_t}
=\frac12\dot M_{\rm crit}c^2
=\boxed{L_{\rm Edd}}.
$$

The [radiative efficiency of black-hole accretion](../../../../../../radiative-efficiency-of-black-hole-accretion.md) therefore decreases inversely with supply rate:

$$
\boxed{\eta=\frac{L}{\dot Mc^2}
\simeq\frac{\dot M_{\rm crit}}{2\dot M}
=\eta_0\frac{\dot M_{\rm Edd}}{\dot M}}.
$$

Order-one coefficients depend on the optical-depth and inner-boundary conventions, but the luminosity saturation and $eta\propto\dot M^{-1}$ are robust.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

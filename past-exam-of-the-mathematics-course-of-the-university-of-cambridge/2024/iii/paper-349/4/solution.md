<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Chandrasekhar dynamical friction](../../../../../chandrasekhar-dynamical-friction.md) is the drag exerted by the overdense gravitational wake that a massive body creates in a background of lighter particles. It transfers orbital energy and [angular momentum](../../../../../angular-momentum.md) to the host, causing satellites, star clusters, and massive black holes to spiral inward and promoting galaxy mergers. In a homogeneous isotropic Maxwellian background its force is

$$
\mathbf F_{\rm df}=-4\pi G^2M^2\rho\log\Lambda
\left[\operatorname{erf}(X)-\frac{2X}{\sqrt\pi}e^{-X^2}\right]
\frac{\mathbf v}{v^3},
\qquad X=\frac{v}{\sqrt2\sigma},
$$

where $\log\Lambda$ is the [Coulomb logarithm in stellar dynamics](../../../../../coulomb-logarithm-in-stellar-dynamics.md). Its scaling can be reconstructed from the strong-deflection [impact parameter](../../../../../impact-parameter.md) $b_{\rm cr}\sim GM/v^2$: the encountered mass rate is $\sim\rho v\pi b_{\rm cr}^2$, and multiplying by momentum change $\sim v$ gives $F_{\rm df}\sim G^2M^2\rho/v^2$.

For a spherical host with a [flat galaxy rotation curve](../../../../../flat-galaxy-rotation-curve.md),

$$
M_h(<r)=\frac{v_c^2r}{G},
\qquad
\rho_h(r)=\frac{v_c^2}{4\pi Gr^2}.
$$

This is a [singular isothermal sphere](../../../../../singular-isothermal-sphere.md) with one-dimensional dispersion $\sigma=v_c/\sqrt2$, so $X=1$. Define

$$
C=\operatorname{erf}(1)-\frac{2e^{-1}}{\sqrt\pi}\simeq0.428.
$$

For a constant-mass satellite on a [circular orbit](../../../../../circular-orbit.md), the drag magnitude and its [torque](../../../../../torque.md) are

$$
F_{\rm df}=\frac{CGM_s^2\log\Lambda}{r^2},
\qquad
\frac{d}{dt}(M_sv_cr)=-rF_{\rm df}.
$$

It follows that

$$
\dot r=-\frac{CGM_s\log\Lambda}{v_cr},
\qquad
\boxed{t_{\rm df,0}=\frac{v_cr_0^2}{2CGM_s\log\Lambda}
\simeq\frac{1.17v_cr_0^2}{GM_s\log\Lambda}}.
$$

The quadratic radius dependence and inverse mass dependence explain why massive nearby satellites merge much faster than light or distant ones.

Let the satellite also have a flat internal rotation curve of speed $v_s$. Equating its edge density to the host density gives the [tidal radius](../../../../../tidal-radius.md)

$$
\frac{v_s^2}{4\pi GR_t^2}=\frac{v_c^2}{4\pi Gr^2},
\qquad
R_t(r)=\frac{v_s}{v_c}r.
$$

Because $M_s(\lt R_t)=v_s^2R_t/G$, the bound mass decreases linearly:

$$
M_s(r)=M_s(r_0)\frac r{r_0}.
$$

Under the question's literal closure that the [derivative](../../../../../derivative.md) of the remaining satellite's total orbital angular momentum equals the frictional torque,

$$
\frac d{dt}\left[M_s(r)v_cr\right]
=-\frac{CGM_s(r)^2\log\Lambda}{r},
$$

and hence

$$
\dot r=-\frac{CGM_s(r_0)\log\Lambda}{2v_cr_0},
\qquad
\boxed{t_{\rm df,strip}=\frac{2v_cr_0^2}{CGM_s(r_0)\log\Lambda}=4t_{\rm df,0}}.
$$

If stripped material is explicitly assigned the satellite's instantaneous specific orbital angular momentum, the balance for the bound remnant is instead $M_s\,d(v_cr)/dt=-rF_{\rm df}$; that convention gives $t_{\rm df,strip}=2t_{\rm df,0}$. Both treatments show the robust point: [tidal stripping](../../../../../tidal-stripping.md) weakens the drag as the orbit shrinks and substantially delays coalescence. In less idealized profiles the mass can fall faster than linearly, producing [dynamical-friction stalling by tidal stripping](../../../../../dynamical-friction-stalling-by-tidal-stripping.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat the morning and evening halves of the [day-night terminator](../../../../../../day-night-terminator.md) as independent, isothermal, hydrostatic atmospheres with the same reference radius $R_0$, reference pressure $P_0$, composition, gravity $g$, and extinction coefficient $\kappa_\lambda$. Their [atmospheric scale heights](../../../../../../atmospheric-scale-height.md) are

$$
H_m=\frac{k_BT_m}{\mu m_Hg},
\qquad
H_e=\frac{k_BT_e}{\mu m_Hg}.
$$

For $H_i\ll R_0$, the slant [optical depth](../../../../../../optical-depth.md) of half $i$ at tangent altitude $z$ is approximately

$$
\tau_{\lambda,i}(z)
=\frac{\kappa_\lambda P_0}{g}
\sqrt{\frac{2\pi R_0}{H_i}}e^{-z/H_i}.
$$

The standard isothermal effective altitude is therefore

$$
z_{\lambda,i}=H_i\left[
\gamma_E+log\left(
\frac{\kappa_\lambda P_0}{g}
\sqrt{\frac{2\pi R_0}{H_i}}
\right)
\right],
$$

up to a wavelength-independent choice of reference radius. The two semicircular limbs add in projected area, so the [exoplanet transmission spectrum](../../../../../../exoplanet-transmission-spectrum.md) is

$$
\boxed{
D_\lambda
=\frac{(R_0+z_{\lambda,m})^2+(R_0+z_{\lambda,e})^2}
{2R_*^2}}.
$$

Equivalently, $R_{\rm tr}^2=[(R_0+z_m)^2+(R_0+z_e)^2]/2$. Differentiating with respect to $\log\kappa_\lambda$ gives

$$
\frac{dR_{\rm tr}}{d\log\kappa_\lambda}
=\frac{(R_0+z_m)H_m+(R_0+z_e)H_e}{2R_{\rm tr}}
\simeq\frac{H_m+H_e}{2}.
$$

Thus a homogeneous retrieval measures, to leading order,

$$
\boxed{H_{\rm av}=\frac{k_B(T_m+T_e)}{2\mu m_Hg}},
$$

provided the opacity and composition do not themselves differ between the two limbs.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 315](../../../paper-315-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

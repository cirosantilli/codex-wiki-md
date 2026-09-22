<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

During a weak encounter, approximate one star's trajectory by a straight line with speed $v$ and [impact parameter](../../../../../../impact-parameter.md) $b$. At longitudinal coordinate $z=vt$, the transverse acceleration is

$$
a_\perp=\frac{Gm b}{(b^2+v^2t^2)^{3/2}}.
$$

Integrating from $t=-\infty$ to $\infty$ gives

$$
\boxed{\delta v_\perp=\frac{2Gm}{bv}
=\frac{2Gm b}{b^2v}}.
$$

Here $Gm/b^2$ sets the gravitational acceleration, $b/v$ is the encounter duration, and the geometric projection produces the displayed transverse impulse.

In one crossing, the number of encounters with impact parameters in $(b,b+db)$ is, up to the system-geometry convention,

$$
dn\simeq\frac{2Nb\,db}{R^2}.
$$

Uncorrelated impulses add in mean square, so

$$
\left\langle(\Delta v)^2\right\rangle_{\rm cross}
=\int_{b_{\min}}^{b_{\max}}(\delta v)^2dn
\simeq\frac{8NG^2m^2}{R^2v^2}
\log\!\frac{b_{\max}}{b_{\min}}.
$$

The [virial theorem](../../../../../../virial-theorem.md) gives $v^2\sim GNm/R$. Taking $b_{\max}\sim R$ and the strong-deflection scale $b_{\min}\sim Gm/v^2\sim R/N$ gives the [Coulomb logarithm in stellar dynamics](../../../../../../coulomb-logarithm-in-stellar-dynamics.md) $\log\Lambda\sim\log N$ and

$$
\frac{\langle(\Delta v)^2\rangle_{\rm cross}}{v^2}
\simeq\frac{8\log\Lambda}{N}.
$$

Velocity memory is lost when the cumulative change reaches $v^2$, after

$$
\boxed{n_{\rm cross}\simeq\frac{N}{8\log\Lambda}
\simeq\frac{N}{8\log N}}.
$$

Consequently the [two-body relaxation](../../../../../../two-body-relaxation.md) time is

$$
\boxed{t_{\rm rel}\simeq\frac{N}{8\log N}\frac{R}{v}},
$$

with an order-unity prefactor depending on density profile and convention. The system is a [collisional stellar system](../../../../../../collisional-stellar-system.md) when $t_{\rm rel}$ is shorter than its age or the evolutionary timescale being studied.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

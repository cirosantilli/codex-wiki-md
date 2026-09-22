<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use [natural units](../../../../natural-units.md) and the [Minkowski metric](../../../../minkowski-metric.md) $g_{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$. Varying the [Proca action](../../../../proca-action.md) with respect to $A_\nu$ gives $\partial\mathcal L/\partial A_\nu=m^2A^\nu$ and $\partial\mathcal L/\partial(\partial_\mu A_\nu)=-F^{\mu\nu}$. The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) is therefore

$$
\boxed{\partial_\mu F^{\mu\nu}+m^2A^\nu=0.}
$$

Taking a divergence annihilates the antisymmetric field strength, since commuting derivatives are symmetric in their indices. For $m\ne0$ this gives the [Lorenz constraint in Proca theory](../../../../lorenz-constraint-in-proca-theory.md) $\partial_\nu A^\nu=0$, and hence $(\Box+m^2)A^\nu=0$. The constraint follows from dynamics; it is not an additional [gauge fixing](../../../../gauge-fixing.md) condition for this massive theory.

For four-[momentum](../../../../momentum-split.md) $p^\mu=(E,0,0,p)$, [longitudinal polarization of a massive vector boson](../../../../longitudinal-polarization-of-a-massive-vector-boson.md) lies in the time–$z$ plane, has $p\cdot\varepsilon=0$ and is normalized by $\varepsilon\cdot\varepsilon=-1$. Taking

$$
\boxed{\varepsilon_L^\mu=\frac1m(p,0,0,E)}
$$

satisfies both requirements because $E^2-p^2=m^2$. It can also be obtained by boosting the rest-frame unit spatial [polarization](../../../../polarization-waves.md) along the direction of motion. Together with two transverse [polarizations](../../../../polarization-waves.md) it gives the three physical spin states of a massive [spin](../../../../spin.md) one particle.

In the [Higgs boson](../../../../higgs-boson.md) rest frame, choose $p^\mu=(E,0,0,p^*)$ and $p'^\mu=(E,0,0,-p^*)$, with $E=m_H/2$ and $p^{*2}=m_H^2/4-m_W^2$. Consistent normalized longitudinal [polarization vectors](../../../../polarization-vector.md) are

$$
\varepsilon_L(p)=\frac1{m_W}(p^*,0,0,E),\qquad
\varepsilon_L(p')=\frac1{m_W}(p^*,0,0,-E).
$$

Their Lorentz contraction is $(p^{*2}+E^2)/m_W^2=(2p^{*2}+m_W^2)/m_W^2$. The [Higgs boson coupling to W bosons](../../../../higgs-boson-coupling-to-w-bosons.md) consequently gives

$$
|\mathcal M_{LL}|^2=\frac{v^2g^4}{4m_W^4}(2p^{*2}+m_W^2)^2
=\frac{m_H^4}{v^2}(1-2x)^2,\qquad x=\frac{m_W^2}{m_H^2}.
$$

Using the [two-body Lorentz-invariant phase space](../../../../two-body-lorentz-invariant-phase-space.md), $p^*=m_H\sqrt{1-4x}/2$ and $v^{-2}=\sqrt2G_F$ yields the longitudinal partial [decay width](../../../../decay-width.md)

$$
\boxed{\Gamma(H\to W_L^+W_L^-)=\frac{G_Fm_H^3}{8\pi\sqrt2}\sqrt{1-4x}\,(1-2x)^2,\qquad m_H>2m_W.}
$$

The charged [W bosons](../../../../w-boson.md) are distinguishable, so there is no identical-particle factor of $1/2$. This expression includes the entire angular phase space but only the specified longitudinal final [polarizations](../../../../polarization-waves.md). The [Higgs decay to two W bosons](../../../../higgs-decay-to-two-w-bosons.md) summed over all [polarizations](../../../../polarization-waves.md) instead has the factor $1-4x+12x^2$; the additional transverse contribution is $8x^2$. At $m_H\gg m_W$ the longitudinal channel dominates and the leading width grows as $G_Fm_H^3$.

<a id="1/image-on-shell-higgs-decay-longitudinal-and-transverse-contributions-to-the-w-pair-width"></a>
![](../../../../past-exam-of-the-gauge-field-theory-course-of-the-university-of-cambridge/2013/paper-1-higgs-ww-polarizations.png)

**[Figure 1](#1/image-on-shell-higgs-decay-longitudinal-and-transverse-contributions-to-the-w-pair-width). On-shell Higgs decay: longitudinal and transverse contributions to the W-pair width**.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the gauge field theory course of the University of Cambridge](../../../split.md)
5. [Gauge Field Theory course of the University of Cambridge](../../../../gauge-field-theory-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)

<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set the external [four-momenta](../../../../../four-momentum.md) to zero after identifying the proper diagrams. In each box or triangle, at least one endpoint of the internal [photon](../../../../../photon.md) is a cubic vertex adjacent to an external scalar of zero [momentum](../../../../../momentum-split.md). That vertex is proportional to $l_\rho$, whereas the supplied numerator obeys $l^\rho P_{\rho\sigma}(l)=0$. All seven such graphs vanish algebraically. This use of the transverse numerator is stronger than merely saying that one has chosen a generic [Lorenz gauge](../../../../../lorenz-gauge-condition.md).

The two surviving [seagull vertex](../../../../../seagull-vertex.md) bubbles have vertex factors $2ie_D^2g^{\mu\rho}$ and $2ie_D^2g^{\sigma\nu}$. Combining their two [propagators](../../../../../propagator.md) gives

$$
\boxed{i\Gamma_{\rm loop}^{\mu\nu}(0)
=-4e_D^4\int\frac{d^Dl}{(2\pi)^D}
\frac{g^{\mu\rho}P_{\rho\sigma}(l)g^{\sigma\nu}}
{(l^2+i0)(l^2-m^2+i0)}+(\mu\leftrightarrow\nu).}
$$

This [scalar-QED four-point vertex pole in transverse gauge](../../../../../scalar-qed-four-point-vertex-pole-in-transverse-gauge.md) calculation determines the proportionality constant as well as the required tensor structure. Keep $m>0$ while extracting the [ultraviolet pole](../../../../../ultraviolet-pole.md). [Lorentz covariance](../../../../../lorentz-covariance.md) inside the regulated integral replaces $l^\mu l^\nu$ by $g^{\mu\nu}l^2/D$, giving the factor $(D-1)g^{\mu\nu}/D$.

For its scalar integral, [Feynman parameter](../../../../../feynman-parameter.md) gives

$$
\begin{aligned}
I_D&=\int\frac{d^Dl}{(2\pi)^D}\frac1{(l^2+i0)(l^2-m^2+i0)}\\
&=\frac{i\Gamma(2-D/2)}{(4\pi)^{D/2}}
\int_0^1 dx\,[(1-x)m^2]^{D/2-2}\\
&=\frac{i\Gamma(2-D/2)(m^2)^{D/2-2}}
{(4\pi)^{D/2}(D/2-1)}
=\frac{i}{8\pi^2\epsilon}+O(1),\qquad D=4-\epsilon.
\end{aligned}
$$

There is no infrared divergence at $l=0$ with nonzero $m$. At pole order the two [photon](../../../../../photon.md) assignments and the factor $3/4$ therefore yield

$$
i\Gamma_{\rm loop}^{\mu\nu}\big|_{\rm pole}
=-\frac{3ie_D^2e^2}{4\pi^2\epsilon}g^{\mu\nu}.
$$

The common engineering scale factor is included in $e_D^2$; finite logarithms are immaterial to the pole. Adding $2ie_D^2\delta_4g^{\mu\nu}$ cancels it when

$$
\boxed{Z_4=1+\frac{3e^2}{8\pi^2\epsilon}+O(e^4)\quad(D=4-\epsilon).}
$$

This is [minimal subtraction scheme](../../../../../minimal-subtraction-scheme.md), up to optional finite terms. It agrees with the transverse-gauge [scalar QED wave-function pole](../../../../../scalar-qed-wave-function-pole.md) and $Z_4=Z_2$. Setting $m=0$ at the outset would instead make the zero-momentum integral scaleless and obscure its separate ultraviolet divergence.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

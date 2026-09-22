<h1 id="section-b/b3/solution">Solution</h1>

↑ **Parent:** [B3](../b3.md)

A [direct band gap](../../../../direct-band-gap.md) has its conduction minimum and valence maximum at the same [crystal momentum](../../../../crystal-momentum.md). A photon can then connect the band-edge states with negligible momentum change. An [indirect band gap](../../../../indirect-band-gap.md) requires an additional phonon to supply or remove momentum, making radiative recombination much less probable. Direct-gap materials such as [gallium arsenide](../../../../gallium-arsenide.md) or [gallium nitride](../../../../gallium-nitride.md) are therefore usually better for a [light-emitting diode](../../../../light-emitting-diode.md) than [silicon](../../../../silicon.md).

For the graded junction, let $q=|e|>0$, $\varepsilon_s=\varepsilon_0\varepsilon_r$, and use electrostatic potential $\varphi$ with $E_x=-\varphi'$. Fully ionized dopants have charge density $\rho=q(N_D-N_A)=q\alpha x$, so [Poisson's equation](../../../../poisson-s-equation.md) is $\varphi''=-q\alpha x/\varepsilon_s$. The paper's displayed plus sign corresponds to using the negative potential $V=-\varphi$, or a signed electron charge in that formula. The positive barrier magnitude and charge magnitude must be used consistently in the width below.

The intended compensation point is **$x=0$**, where $N_D=N_A$ and the net doping changes sign. A locally neutral model with comparable electron and hole mobilities has its lowest carrier conductivity near there. The [depletion approximation](../../../../depletion-approximation.md) neglects mobile-carrier conductivity throughout the layer, so it does not by itself locate an exact conductivity minimum; unequal mobilities or asymmetric carrier profiles can shift it.

Let the depletion edges be $x=\pm d$. With zero exterior field, integrating $E_x'=\rho/\varepsilon_s$ and imposing $E_x(\pm d)=0$ gives the [linearly graded p-n junction](../../../../linearly-graded-p-n-junction.md) field

$$
\boxed{E_x(x)=\frac{q\alpha}{2\varepsilon_s}(x^2-d^2),\qquad |E_x|_{\max}=\frac{q\alpha d^2}{2\varepsilon_s}\text{ at }x=0.}
$$

Its integral gives $\varphi(x)=\varphi(0)+q\alpha(d^2x-x^3/3)/(2\varepsilon_s)$, so the [electric potential](../../../../electric-potential.md) increases toward the n-type side while the electron band edges $E_c,E_v$ bend downward together. Their separation is the local band gap, and the equilibrium [electrochemical potential](../../../../electrochemical-potential.md) is flat. The [built-in potential](../../../../built-in-potential.md) arises when carrier diffusion exposes ionized dopants until the opposing field balances further diffusion.

<a id="section-b/b3/image-band-bending-and-electric-field-in-a-symmetric-linearly-graded-junction"></a>
![](../../../../past-exam-of-the-quantum-condensed-matter-course-of-the-university-of-cambridge/2007-graded-junction.png)

**[Figure 3](#section-b/b3/image-band-bending-and-electric-field-in-a-symmetric-linearly-graded-junction). Band bending and electric field in a symmetric linearly graded junction**. Original schematic band edges and a flat equilibrium chemical potential. The lower panel plots the normalized parabolic depletion field; outside the edges it is zero. Energy offsets are illustrative, while the cubic potential and field shape follow from the graded-charge model.

Finally the positive barrier is

$$
V_b=\varphi(d)-\varphi(-d)=-\int_{-d}^dE_x\,dx=\frac{2q\alpha d^3}{3\varepsilon_s}.
$$

With total width $w=2d$, this yields the [linearly graded junction depletion width](../../../../linearly-graded-junction-depletion-width.md)

$$
\boxed{w=\left(\frac{12\varepsilon_0\varepsilon_rV_b}{q\alpha}\right)^{1/3}.}
$$

Here $\alpha>0$ labels p-to-n progression with increasing $x$; otherwise use its magnitude in the width formula.

## ↑ Ancestors (13)

1. [B3](../b3.md)
2. [Section B](../../section-b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../split.md)
5. [Quantum Condensed Matter course of the University of Cambridge](../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)

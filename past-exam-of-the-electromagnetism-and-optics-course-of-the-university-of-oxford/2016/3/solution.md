<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take $d$ as the centre-to-centre separation and $\epsilon=\epsilon_0\epsilon_r$. Use the ideal lossless two-conductor [transmission line](../../../transmission-line.md) model, with nonmagnetic surroundings and negligible internal-wire [inductance](../../../inductance.md). Opposite [line charges](../../../line-charge.md) $+\lambda_q$ and $-\lambda_q$ approximate the cylindrical conductors when $d\gg a$. Integrating their [electric fields](../../../electric-field-split.md), or adding their logarithmic [electric potentials](../../../electric-potential.md), gives the potential difference

$$
V\simeq\frac{\lambda_q}{\pi\epsilon}\ln\frac da,
\qquad C'=\frac{\lambda_q}{V}\simeq\frac{\pi\epsilon}{\ln(d/a)}.
$$

This is the [two-wire capacitance at large separation](../../../two-wire-capacitance-at-large-separation.md). For opposite [electric currents](../../../electric-current.md) $+I$ and $-I$, the [magnetic fields](../../../magnetic-field-split.md) between the wires add. The linked [magnetic flux](../../../magnetic-flux.md) per unit length is approximately

$$
\Phi'\simeq\frac{\mu_0I}{2\pi}\int_a^{d-a}\left(\frac1x+\frac1{d-x}\right)dx
=\frac{\mu_0I}{\pi}\ln\frac{d-a}{a}
\simeq\frac{\mu_0I}{\pi}\ln\frac da.
$$

Thus the [external inductance of a thin two-wire line](../../../external-inductance-of-a-thin-two-wire-line.md) is $L'\simeq\mu_0\ln(d/a)/\pi$. The lossless [telegrapher's equations](../../../telegrapher-s-equations.md) give a forward [wave](../../../wave-split.md) with $V/I=\sqrt{L'/C'}$, so its [characteristic impedance](../../../characteristic-impedance.md) is

$$
\boxed{Z_0\simeq\frac1\pi\sqrt{\frac{\mu_0}{\epsilon_0\epsilon_r}}\ln\frac da
\simeq\frac{120\,\Omega}{\sqrt{\epsilon_r}}\ln\frac da.}
$$

The product $L'C'=\mu_0\epsilon$ also gives the propagation speed $c/\sqrt{\epsilon_r}$, an independent consistency check. The exact ideal external-field geometry replaces $\ln(d/a)$ by $\operatorname{arcosh}(d/(2a))$. If the wire separation were specified between surfaces, its centre separation would be $d+2a$, with the same leading large-separation result. Finite [electrical conductivity](../../../electrical-conductivity.md) and internal-wire [magnetic energy](../../../magnetic-energy.md) require a more detailed line model.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2016](../../2016-split.md)
3. [Past exam of the electromagnetism and optics course of the University of Oxford](../../split.md)
4. [Electromagnetism and optics course of the University of Oxford](../../../electromagnetism-and-optics-course-of-the-university-of-oxford.md)
5. [Year 2 of the physics course of the University of Oxford](../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

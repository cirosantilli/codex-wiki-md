<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In the [adiabatic cloud droplet number retrieval](../../../../adiabatic-cloud-droplet-number-retrieval.md), the independently retrieved [liquid-water path](../../../../liquid-water-path.md) fixes the geometrical thickness in the adiabatic model:

$$
W=\int_0^Hw(h)\,dh=\tfrac12c_wH^2,
\qquad \boxed{H=(2W/c_w)^{1/2}.}
$$

Define $C_c=(3/5)\pi Q_{\rm ext}k^{1/3}[3c_w/(4\pi\rho_w)]^{2/3}$. Since $\tau_c=C_cN^{1/3}H^{5/3}$, eliminating $H$ gives

$$
\boxed{N=\left(\frac{\tau_c}{C_c}\right)^3
\left(\frac{c_w}{2W}\right)^{5/2}
=\frac{250\sqrt2}{243\pi Q_{\rm ext}^3k}\,
\rho_w^2c_w^{1/2}\frac{\tau_c^3}{W^{5/2}}.}
$$

Use SI units to obtain $N$ in $\mathrm{m^{-3}}$, then divide by $10^6$ for $\mathrm{cm^{-3}}$. The sensitivity is substantial: $d\log N=3d\log\tau_c-(5/2)d\log W+(1/2)d\log c_w-d\log k-3d\log Q_{\rm ext}$. Thus a numerical retrieval additionally needs the adiabatic [condensation](../../../../condensation.md) coefficient, [shape factor](../../../../adiabatic-cloud-droplet-moments.md) and [extinction](../../../../particle-extinction-coefficient.md) efficiency. A nonadiabatic water profile, mixed phase, horizontal inhomogeneity or a biased water-path retrieval can produce a large number-concentration bias.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

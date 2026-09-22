<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A regulator and a [renormalization condition](../../../../../renormalization-condition.md) introduce the reference mass scale $\mu$, even when the classical theory has no mass. Loop amplitudes contain dimensionless logarithms of momentum or distance ratios involving $\mu$. The resulting [running coupling](../../../../../running-coupling.md) and field normalization compensate changes of this arbitrary reference scale.

Let $\phi_0=Z_\phi^{1/2}\phi$ and $G_n=Z_\phi^{-n/2}G_{n,0}$. Hold the bare parameters fixed and define $\beta(g)=\mu\,dg/d\mu$ and $\gamma(g)=\frac12\mu\,d\log Z_\phi/d\mu$. Assuming multiplicative field [renormalization](../../../../../renormalization.md) and no mixing or additive contact terms for the correlator, differentiating gives the [Callan-Symanzik equation](../../../../../callan-symanzik-equation.md)

$$
\boxed{(\mu\partial_\mu+\beta(g)\partial_g+n\gamma(g))G_n=0.}
$$

For the dimensionless two-point factor put $r=p^2/\mu^2$. Its equation is $(-2r\partial_r+\beta\partial_g+2\gamma)C=0$. Let

$$
\frac{dg(t)}{dt}=\beta(g(t)),\quad g(0)=g,\qquad f(t)=\exp\left(2\int_0^t\gamma(g(u))\,du\right).
$$

The [characteristic solution of the multiplicative Callan-Symanzik equation](../../../../../characteristic-solution-of-the-multiplicative-callan-symanzik-equation.md) is

$$
\boxed{C(e^{2t}r,g)=f(t)C(r,g(t)).}
$$

To check the sign, $\partial_tC(e^{2t}r,g)=2e^{2t}r\partial_rC$ equals $(\beta\partial_g+2\gamma)C$. The characteristic flow and its accumulated multiplier give precisely this evolution. Changing $\mu$ changes the dimensionless momentum and renormalized $g$; the same bare [two-point correlation function](../../../../../two-point-correlation-function.md) is recovered after the compensating field normalization. An unnormalized renormalized correlator need not remain numerically identical under that change, but physical predictions do.

With a mass, write $v=m/\mu$ and define its [running mass](../../../../../running-mass.md) by $m'(t)=\delta(g(t))m(t)$, $m(0)=m$. The dimensionless equation becomes

$$
[-2r\partial_r+\beta\partial_g+(\delta-1)v\partial_v+2\gamma]C=0.
$$

Its flow is therefore

$$
\boxed{C(e^{2t}r,m/\mu,g)=f(t)C(r,e^{-t}m(t)/\mu,g(t)),\quad m(t)=m\exp\left(\int_0^t\delta(g(u))\,du\right).}
$$

The [renormalization-group mass suppression criterion](../../../../../renormalization-group-mass-suppression-criterion.md) is $\int_0^t(\delta(g(u))-1)du\to-\infty$, for example an eventual bound $\delta\le1-\eta$ with $\eta>0$. Then the mass argument on the right tends to zero. A regular [massless limit](../../../../../massless-limit.md), uniform along the limiting coupling trajectory, makes the mass negligible at high energies. Merely calling $\delta$ small without controlling this integrated exponent is insufficient.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the dense current lies on the bottom, $\Delta\rho>0$, and its height is small compared with the confined aquifer depth $w$. This permits the [hydrostatic approximation](../../../../../../hydrostatic-approximation.md) and neglect of leading-order resistance from the return flow of the original fluid. The dense-layer pressure anomaly on the basal seal is $\Delta\rho gh$. The along-layer [Darcy flux](../../../../../../darcy-velocity.md), integrated over the current thickness, and the downward leakage flux are respectively

$$
q_x=-\frac{k\Delta\rho g}{\mu}h h_x,
\qquad q_\ell=\frac{\lambda\Delta\rho g}{\mu b}h.
$$

[Volume conservation](../../../../../../volume-conservation.md) requires $\phi h_t+\partial_xq_x=-q_\ell$. Thus the [porous gravity current](../../../../../../porous-gravity-current.md) with [hydrostatic leakage through a basal seal](../../../../../../hydrostatic-leakage-through-a-basal-seal.md) obeys

$$
\boxed{h_t=D(hh_x)_x-\Omega h,
\quad D=\frac{k\Delta\rho g}{\phi\mu},
\quad\Omega=\frac{\lambda\Delta\rho g}{\phi\mu b}.}
$$

Here [permeability of a porous medium](../../../../../../permeability-of-a-porous-medium.md) has units of area, and $\Omega$ has units of inverse time. The original PDF instead prints the sink coefficient $\lambda k\Delta\rho g/(\mu b)$. With $\lambda$ defined there as a permeability, that coefficient has units of area per time and cannot multiply $h$ to give $h_t$. It also omits the division of leakage by [porosity](../../../../../../porosity.md). This is a genuine source error, not a [Darcy law](../../../../../../darcy-law.md) convention. The remaining parts solve the stated linear-drainage equation for a constant $\Omega>0$; the physically consistent coefficient is the one above. Formally treating the printed coefficient as an independently prescribed inverse-time constant leaves those mathematical solutions unchanged.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

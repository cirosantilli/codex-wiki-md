<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Differentiate the product of [Dirac delta functions](../../../../../../dirac-delta-function.md) defining $\widetilde P$, regarding $B$ and $\sigma$ as independent density arguments. The random continuity equation is

$$
\partial_t\widetilde P=-\partial_B(\sigma B\widetilde P)+\frac1\tau\partial_\sigma(\sigma\widetilde P)-\partial_\sigma(f\widetilde P).
$$

For $0<s<t$, the causal [functional derivatives](../../../../../../functional-derivative.md) follow from the explicit strain solution and $\widetilde B(t)=B_0\exp[\int_0^t\widetilde\sigma(u)\,du]$:

$$
\frac{\delta\widetilde\sigma(t)}{\delta f(s)}=e^{-(t-s)/\tau},\qquad \frac{\delta\widetilde B(t)}{\delta f(s)}=\widetilde B(t)\tau\left[1-e^{-(t-s)/\tau}\right].
$$

Consequently,

$$
\frac{\delta\widetilde P(t)}{\delta f(s)}=-e^{-(t-s)/\tau}\partial_\sigma\widetilde P-\tau\left[1-e^{-(t-s)/\tau}\right]\partial_B(\widetilde B(t)\widetilde P).
$$

In the [Furutsu–Novikov formula](../../../../../../novikov-s-theorem.md), the covariance $\kappa\delta(t-s)$ samples the upper endpoint of the causal time integral. Symmetric regularization of the [white noise](../../../../../../white-noise.md) gives half the mass there. The $B$ response vanishes as $s\uparrow t$, while the strain response tends to one, so $\mathbb E[f(t)\widetilde P(t)]=-(\kappa/2)\partial_\sigma P$. Averaging the continuity equation yields the [Fokker-Planck equation](../../../../../../fokker-planck-equation.md)

$$
\boxed{\partial_tP=-\partial_B(\sigma BP)+\frac1\tau\partial_\sigma(\sigma P)+\frac\kappa2\partial_\sigma^2P.}
$$

There is no direct diffusion term in $B$: its equation contains the time integral of [colored noise](../../../../../../colored-noise.md), whereas the strain equation receives [Gaussian white noise](../../../../../../gaussian-white-noise.md). The same result follows from the [Itô diffusion](../../../../../../ito-diffusion.md) with drift $(\sigma B,-\sigma/\tau)$ and diffusion vector $(0,\sqrt\kappa)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

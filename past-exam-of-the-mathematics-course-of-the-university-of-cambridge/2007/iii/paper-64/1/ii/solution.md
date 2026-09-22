<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Retain the homogeneous [lapse function](../../../../../../lapse-function.md) $\bar N(t)$, and define the physical [Hubble parameter](../../../../../../hubble-parameter.md) $H=\dot a/(\bar Na)$. At first order the scalar [metric perturbations](../../../../../../linearized-gravity.md) give $\delta g_{00}=-2\bar N^2\Phi$, $\delta g_{0i}=a^2B_{,i}$, and $\delta g_{ij}=-2a^2(\Psi\delta_{ij}+E_{,ij})$. Applying the passive coordinate displacement component by component gives the [scalar gauge transformations with a background lapse](../../../../../../scalar-gauge-transformations-with-a-background-lapse.md)

$$
\boxed{\widetilde\Phi=\Phi-\dot\xi^0-\frac{\dot{\bar N}}{\bar N}\xi^0,\quad
\widetilde B=B-\dot\lambda+\frac{\bar N^2}{a^2}\xi^0,\quad
\widetilde\Psi=\Psi+\frac{\dot a}{a}\xi^0,\quad
\widetilde E=E+\lambda.}
$$

For example the $0i$ transformation is $\delta\widetilde g_{0i}=a^2\partial_iB-a^2\partial_i\dot\lambda+\bar N^2\partial_i\xi^0$. The spatial isotropic part acquires $-2a\dot a\xi^0\delta_{ij}$, explaining the positive sign in the transformation of $\Psi$.

Preserving [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md) requires both transformed $\Phi$ and $B$ to remain zero. The first condition is $\partial_t(\bar N\xi^0)=0$, and the second is $\dot\lambda=\bar N^2\xi^0/a^2$. Integrating them gives

$$
\boxed{\xi^0=\frac{C(\mathbf x)}{\bar N},\qquad
\lambda=C(\mathbf x)\int^t\frac{\bar N(t')}{a(t')^2}dt'+D(\mathbf x).}
$$

Thus fixing the [lapse function](../../../../../../lapse-function.md) and [shift vector](../../../../../../shift-vector.md) perturbations does not exhaust the scalar coordinate freedom. The functions $C,D$ describe [residual synchronous-gauge freedom](../../../../../../residual-synchronous-gauge-freedom.md); an integration-origin change in the integral is absorbed into $D$.

To move from [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md) to [Newtonian gauge](../../../../../../newtonian-gauge.md), choose $\lambda=-E_S$ to set $\widetilde E=0$. Requiring $\widetilde B=0$ then gives

$$
\xi^0=-\frac{a^2}{\bar N^2}\dot E_S.
$$

A scalar [energy density](../../../../../../energy-density.md) transforms as $\delta\rho_N=\delta\rho_S-\dot{\bar\rho}\xi^0$. Dividing by the background [energy density](../../../../../../energy-density.md), which changes the contrast only at second order if perturbed in that denominator, yields the [synchronous-to-Newtonian density transformation with a lapse](../../../../../../synchronous-to-newtonian-density-transformation-with-a-lapse.md)

$$
\boxed{\delta_N=\delta_S+\frac{a^2\dot E_S}{\bar N^2}\frac{\dot{\bar\rho}}{\bar\rho}
=\delta_S-3(1+w)\frac{a^2H}{\bar N}\dot E_S,
\qquad\delta=\frac{\delta\rho}{\bar\rho}.}
$$

The last form uses background [stress-energy conservation](../../../../../../stress-energy-conservation.md), $\dot{\bar\rho}=-3\bar NH(\bar\rho+\bar P)$. With [cosmic time](../../../../../../cosmic-time.md) $\bar N=1$ this is $\delta_N=\delta_S-3(1+w)a^2H\dot E_S$; with [conformal time](../../../../../../conformal-time.md) $\bar N=a$ it is $\delta_N=\delta_S-3(1+w)\mathcal H E_S'$, where $\mathcal H=a'/a$. Keeping these clock conventions distinct is essential to the factors of $a$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

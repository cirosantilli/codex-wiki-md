<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Normalize today's [scale factor](../../../../../../scale-factor-cosmology.md) to $a_0=1$ and use $c=1$. A source of bolometric [luminosity](../../../../../../luminosity.md) $L$ emits [photons](../../../../../../photon.md) whose [energies](../../../../../../energy.md) arrive smaller by $1+z$, and whose arrival intervals are longer by $1+z$. Their wavefront has physical area $4\pi a_0^2r_1^2$. The received [radiative flux](../../../../../../radiative-flux.md) is therefore

$$
F=\frac{L}{4\pi a_0^2r_1^2(1+z)^2}.
$$

By the definition of [luminosity distance](../../../../../../luminosity-distance.md), $F=L/(4\pi d_L^2)$, so $d_L=(1+z)a_0r_1=r_1/a_{\rm em}$. The final equality assumes the stated normalization of the [scale factor](../../../../../../scale-factor-cosmology.md); it is not a formula invariant under an arbitrary rescaling of $a_0$.

A radial [null geodesic](../../../../../../null-geodesic.md) of the [FRW metric](../../../../../../friedmann-lemaitre-robertson-walker-metric.md) obeys $dt/a=dr/\sqrt{1-Kr^2}$. Using $1+z=1/a$ and $dz/dt=-(1+z)H(z)$ gives the radial [comoving distance](../../../../../../comoving-radial-distance.md)

$$
\chi(z)=\int_{t_{\rm em}}^{t_0}\frac{dt}{a(t)}
=\int_0^z\frac{dz'}{H(z')}
=\int_0^{r_1}\frac{dr}{\sqrt{1-Kr^2}}.
$$

For $K>0$ this last integral is $\arcsin(\sqrt K r_1)/\sqrt K$, continued along the radial coordinate when necessary; for $K<0$ it is $\operatorname{arsinh}(\sqrt{|K|}r_1)/\sqrt{|K|}$. Inverting, with $\Omega_K=-K/H_0^2$, proves

$$
\boxed{d_L(z)=\frac{1+z}{H_0\sqrt{|\Omega_K|}}\,
S_K\!\left(H_0\sqrt{|\Omega_K|}\int_0^z\frac{dz'}{H(z')}\right).}
$$

Here $S_K$ is sine for positive [spatial curvature of an FLRW universe](../../../../../../spatial-curvature-of-an-flrw-universe.md), hyperbolic sine for negative [spatial curvature of an FLRW universe](../../../../../../spatial-curvature-of-an-flrw-universe.md), and its argument for zero [spatial curvature of an FLRW universe](../../../../../../spatial-curvature-of-an-flrw-universe.md). The flat case is the continuous limit $d_L=(1+z)\chi$, not a literal division by zero. The original PDF has $H_0\sqrt{|\Omega_K|}$ in the denominator and $H=\dot a/a$; the converted TeX loses these details.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

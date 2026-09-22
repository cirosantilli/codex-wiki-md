<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a fixed coordinate cell, the spatial volume element is

$$
\sqrt{\det g_{ij}}\,d^3x=a^3\sqrt{\det(\delta_{ij}+h_{ij})}\,d^3x
=a^3(1+\tfrac12h)d^3x+O(h^2).
$$

Thus its perturbation relative to the background expansion, or its perturbed [comoving volume](../../../../../../comoving-volume.md), is $\Delta V_c/V_c=h/2$. In the cold-matter rest frame each such cell contains a fixed amount of matter. Since density is mass divided by physical volume,

$$
\boxed{\delta_c=-\frac{\Delta V_c}{V_c}=-\frac h2.}
$$

Equivalently, [stress-energy conservation](../../../../../../stress-energy-conservation.md) gives $\delta_c'=-h'/2$; the stated relation fixes the spatially dependent integration constant by the initial mass-coordinate convention. A contraction of [comoving volume](../../../../../../comoving-volume.md) gives a positive [density contrast](../../../../../../density-contrast.md).

In the matter era $a\propto\tau^2$, so $\mathcal H=2/\tau$ and the matter density fraction is approximately one. The evolution equation reduces to

$$
\delta_c''+\frac2\tau\delta_c'-\frac6{\tau^2}\delta_c=0.
$$

For $\delta_c\propto\tau^p$, the indicial equation is $p(p-1)+2p-6=(p-2)(p+3)=0$. Therefore

$$
\boxed{\delta_c(\mathbf k,\tau)=C_+(\mathbf k)\tau^2+C_-(\mathbf k)\tau^{-3}.}
$$

The growing mode is proportional to $a$, and the decaying mode to $a^{-3/2}$. These are the density solutions after the comoving coordinate choice; the residual time mode found in part (i) explains why a similar power in an unfixed density variable cannot be interpreted in isolation.

There is a normalization omission in the printed density parameter if $\bar\rho_c$ denotes physical density. Its usual definition in [conformal time](../../../../../../conformal-time.md) is

$$
\Omega_c=\frac{8\pi G\bar\rho_c}{3H^2}=\frac{8\pi G a^2\bar\rho_c}{3\mathcal H^2},\qquad H=\frac{a'}{a^2}.
$$

The printed expression lacks $a^2$, unless its density is already rescaled by that factor. The matter-era statement $\Omega_c\simeq1$ and the growth equation use the physical density fraction above.

On [superhorizon scales](../../../../../../superhorizon-scale.md) during [radiation domination](../../../../../../radiation-domination.md), the regular [adiabatic cosmological perturbation](../../../../../../adiabatic-initial-conditions.md) has approximately constant primordial curvature. The comoving density perturbation is gradient-suppressed, of order $(k/\mathcal H)^2$ times that curvature. Since $\mathcal H\propto\tau^{-1}$, it grows as $\delta_c\propto k^2\tau^2$ for fixed mode amplitude. This is the regular superhorizon solution in the specified slicing, not causal collapse driven by communication across the entire wavelength.

After radiation-era horizon entry, the dominant radiation develops pressure-supported acoustic oscillations. Its potential no longer provides a steady growing gravitational source, while cold matter is too small a fraction of the total density to produce rapid self-gravitating growth. The result is the [Mészáros effect](../../../../../../meszaros-effect.md): growth is strongly suppressed until equality. The supplied stagnation approximation replaces that slow evolution by a constant. More accurately, ignoring the rapidly oscillating source at leading order gives $\delta_c''+\delta_c'/\tau\simeq0$, with a constant and a logarithmic solution. Thus **radiation-era subhorizon growth is at most slow logarithmic growth, rather than the matter-era power law**; treating it as constant is the explicit approximation used for the simple transfer estimate below.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

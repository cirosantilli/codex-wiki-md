<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Use the total [density of states](../../../../density-of-states.md) $D^*=Am^*/(2\pi\hbar^2)$ and $C=A/(2\pi\hbar)^2$ from part (b). In the paper's double-sum convention, $f(\phi)$ has units of [energy](../../../../energy-split.md) and scales as $A^{-1}$. Define its first angular moment by

$$
\overline f_1=\int_0^{2\pi}\frac{d\phi}{2\pi}\,f(\phi)\cos\phi.
$$

This convention matters: the [Landau quasiparticle energy functional](../../../../landau-quasiparticle-energy-functional.md) written with an explicit $1/A$ instead uses the intensive kernel $\widetilde f=Af$.

At zero [temperature](../../../../temperature-split.md), the displayed functional is the change in $E-\mu N$; a true [Galilean boost](../../../../galilean-transformation.md) preserves $N$, so $\Delta\mathcal F=\Delta E$. For a radial displacement $\nu(\theta)$, the first term in the [Landau quasiparticle energy functional](../../../../landau-quasiparticle-energy-functional.md) becomes

$$
\begin{aligned}
\Delta\mathcal F_{\rm qp}
&=C\int_0^{2\pi}d\theta\int_{p_F}^{p_F+\nu(\theta)}p\,dp\,\frac{p_F}{m^*}(p-p_F)\\
&=\frac{Cp_F^2}{2m^*}\int_0^{2\pi}\nu(\theta)^2\,d\theta+o(p_0^2).
\end{aligned}
$$

The oriented radial [integral](../../../../integral-split.md) also works for negative $\nu$: removing occupied levels below the [chemical potential](../../../../chemical-potential-split.md) costs positive [energy](../../../../energy-split.md). Substituting $\nu=p_0\cos\theta+O(p_0^2/p_F)$ and using $N=C\pi p_F^2$ gives

$$
\boxed{\Delta\mathcal F_{\rm qp}=\frac{Np_0^2}{2m^*}+o(p_0^2).}
$$

The exact second-order correction to the boundary is unnecessary here because the unperturbed excitation [energy](../../../../energy-split.md) vanishes on the [Fermi surface](../../../../fermi-surface.md); it changes this term only beyond quadratic order. It must nevertheless be understood when identifying $\Delta\mathcal F$ with a fixed-[particle number](../../../../particle-number.md) [energy](../../../../energy-split.md) change.

For the quadratic interaction term, the first-order occupation change alone suffices. The radial [Dirac delta function](../../../../dirac-delta-function.md) integrals give

$$
\Delta\mathcal F_{\rm int}=\frac{C^2p_F^2p_0^2}{2}
\int_0^{2\pi}d\theta\int_0^{2\pi}d\theta'\,
f(\theta-\theta')\cos\theta\cos\theta'+o(p_0^2).
$$

Put $\phi=\theta-\theta'$. The remaining angular [integral](../../../../integral-split.md) uses

$$
\int_0^{2\pi}\cos(\theta'+\phi)\cos\theta'\,d\theta'=\pi\cos\phi,
$$

so only the first cosine component of the interaction survives. Since $D^*=2\pi Cm^*$,

$$
\begin{aligned}
\Delta\mathcal F_{\rm int}
&=\frac{C^2p_F^2p_0^2\pi}{2}\int_0^{2\pi}f(\phi)\cos\phi\,d\phi+o(p_0^2)\\
&=\frac{Np_0^2}{2m^*}\,D^*\overline f_1+o(p_0^2).
\end{aligned}
$$

Adding both contributions and matching the bare-[mass](../../../../mass.md) result of part (a) yields the [two-dimensional Landau effective-mass relation](../../../../two-dimensional-landau-effective-mass-relation.md):

$$
\boxed{\Delta E=\frac{Np_0^2}{2m^*}\left(1+D^*\overline f_1\right)+o(p_0^2),\qquad
\frac{m^*}{m}=1+D^*\int_0^{2\pi}\frac{d\phi}{2\pi}\,f(\phi)\cos\phi.}
$$

Equivalently, using the [density of states](../../../../density-of-states.md) per unit area $g^*=D^*/A$,

$$
\boxed{\frac{m^*}{m}=1+g^*\int_0^{2\pi}\frac{d\phi}{2\pi}\,\widetilde f(\phi)\cos\phi.}
$$

If dimensionless [Landau parameters](../../../../landau-parameter.md) are defined through the [Fourier series](../../../../fourier-series-split.md) $D^*f(\phi)=F_0+\sum_{\ell\geq1}F_\ell\cos(\ell\phi)$, then $D^*\overline f_1=F_1/2$ and

$$
\boxed{\frac{m^*}{m}=1+\frac{F_1}{2}.}
$$

Defining the cosine expansion with an extra factor of two would instead absorb that factor into $F_1$; the angular-[integral](../../../../integral-split.md) formula above fixes the convention unambiguously. The physical content is that interaction changes accompanying a moving [Fermi sea](../../../../fermi-sea.md) compensate the renormalized [quasiparticle](../../../../quasiparticle.md) [velocity](../../../../velocity.md), so the total boost [energy](../../../../energy-split.md) is governed by the bare [mass](../../../../mass.md). For an interaction independent of angle, $\overline f_1=0$ and this consistency condition requires $m^*=m$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the quantum matter course of the University of Oxford](../../../split.md)
5. [Quantum matter course of the University of Oxford](../../../../quantum-matter-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

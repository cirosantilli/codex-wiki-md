<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume nondegenerate three-dimensional parabolic band edges, a fixed gap and approximately temperature-independent density-of-states effective masses. Let $\mu$ be the [chemical potential](../../../../chemical-potential-split.md), $E_c$ and $E_v$ the band edges, and $N_c,N_v$ their [effective density of states](../../../../effective-density-of-states.md). Boltzmann occupation gives

$$
n=N_c e^{-(E_c-\mu)/(k_BT)},\qquad
p=N_v e^{-(\mu-E_v)/(k_BT)},\qquad E_g=E_c-E_v.
$$

For one spin-degenerate spherical conduction extremum, direct integration of $g_c(E)\propto\sqrt{E-E_c}$ gives

$$
N_c=2\left(\frac{m_c^*k_BT}{2\pi\hbar^2}\right)^{3/2},
$$

and similarly for the [valence band](../../../../valence-band.md) with its appropriate density-of-states [mass](../../../../mass.md). Valley and additional band degeneracies can be included in these prefactors. The $T^{3/2}$ factor follows from the integral $\int_0^\infty\sqrt\epsilon\,e^{-\epsilon/(k_BT)}d\epsilon\propto T^{3/2}$.

Multiplication removes the [chemical potential](../../../../chemical-potential-split.md):

$$
np=N_cN_v e^{-E_g/(k_BT)}.
$$

The [semiconductor mass-action law](../../../../semiconductor-mass-action-law.md) combined with intrinsic [charge neutrality](../../../../charge-neutrality.md), $n=p$, therefore gives

$$
\boxed{n_i=\sqrt{N_cN_v}\,e^{-E_g/(2k_BT)}=AT^{3/2}e^{-E_g/(2k_BT)}}.
$$

The intrinsic [chemical potential](../../../../chemical-potential-split.md) is not necessarily exactly midgap: $\mu_i=(E_c+E_v)/2+(k_BT/2)\ln(N_v/N_c)$. Equal effective masses are unnecessary for the displayed carrier-density law. A changing gap, effective [mass](../../../../mass.md) or degeneracy would make the prefactor or activation law [temperature](../../../../temperature-split.md) dependent.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

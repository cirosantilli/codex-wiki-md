<h1 id="section-c/c8/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Keep the [electron](../../../../../../electron.md) number fixed, so

$$
N_e=\int_0^\infty g(\epsilon)p_F(\epsilon)\,d\epsilon
$$

and $\mu(0)=E_F$. Heating smooths the [Fermi-Dirac distribution](../../../../../../fermi-dirac-distribution.md) across the [Fermi energy](../../../../../../fermi-energy.md), creating holes below $\mu$ and particles above it. The sign of the low-[temperature](../../../../../../temperature-split.md) adjustment of [chemical potential](../../../../../../chemical-potential-split.md) follows from the local slope of the [density of states](../../../../../../density-of-states.md).

In one dimension, $g\propto\epsilon^{-1/2}$ decreases with [energy](../../../../../../energy-split.md). At fixed $\mu$, smoothing removes more [electrons](../../../../../../electron.md) below it than it adds above it, so $\mu$ initially rises. In three dimensions, $g\propto\epsilon^{1/2}$ increases, so $\mu$ falls. In two dimensions the constant [density of states](../../../../../../density-of-states.md) makes the leading changes cancel, so $\mu$ stays extremely close to $E_F$ in the degenerate regime.

For quantitative checks, a [Sommerfeld expansion](../../../../../../sommerfeld-expansion.md) gives, for $k_BT\ll E_F$,

$$
\boxed{\mu_1(T)=E_F+\frac{\pi^2}{12}\frac{(k_BT)^2}{E_F}+\cdots,\qquad
\mu_3(T)=E_F-\frac{\pi^2}{12}\frac{(k_BT)^2}{E_F}+\cdots.}
$$

For a constant two-dimensional [density of states](../../../../../../density-of-states.md) above an unbounded parabolic band bottom, the number [integral](../../../../../../integral-split.md) can be done exactly:

$$
N_e=g_2k_BT\ln(1+e^{\mu_2/(k_BT)})=g_2E_F,
$$

so

$$
\boxed{\mu_2(T)=k_BT\ln\left(e^{E_F/(k_BT)}-1\right)
=E_F+k_BT\ln\left(1-e^{-E_F/(k_BT)}\right).}
$$

It actually decreases, but its low-[temperature](../../../../../../temperature-split.md) correction is exponentially small rather than quadratic. “Constant in two dimensions” is therefore a low-[temperature](../../../../../../temperature-split.md) approximation, not an exact statement for every $T$.

The one-dimensional rise is also only an initial trend. In the high-[temperature](../../../../../../temperature-split.md) [Maxwell-Boltzmann distribution](../../../../../../maxwell-boltzmann-distribution.md) limit, the ideal $d$-dimensional [electron gas](../../../../../../electron-gas.md) has $\mu\simeq k_BT\ln[n_d\lambda_T^d/2]$, where $n_d=N_e/L^d$ and $\lambda_T=\sqrt{2\pi\hbar^2/(mk_BT)}$ is the [thermal de Broglie wavelength](../../../../../../thermal-de-broglie-wavelength.md). It eventually becomes negative and decreases in every dimension. The one-dimensional [chemical potential](../../../../../../chemical-potential-split.md) thus passes through a maximum. This high-[temperature](../../../../../../temperature-split.md) statement refers to the stipulated unbounded free-electron [dispersion relation](../../../../../../dispersion-relation-split.md), not a claim that a real finite-width crystal band remains parabolic indefinitely.

## ↑ Ancestors (15)

1. [F](../f.md)
2. [C8](../../c8.md)
3. [Section C](../../../section-c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the physics A course of the University of Cambridge](../../../../../split.md)
7. [Physics A course of the University of Cambridge](../../../../../../physics-a-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)

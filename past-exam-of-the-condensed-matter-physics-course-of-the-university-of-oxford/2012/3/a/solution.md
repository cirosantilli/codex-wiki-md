<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume [thermal equilibrium](../../../../thermal-equilibrium-split.md), nondegenerate carriers, and isotropic [parabolic band dispersions](../../../../parabolic-band-dispersion.md), with the supplied [effective masses](../../../../band-effective-mass.md) interpreted as density-of-states masses. Take one effective valley with two [electron spin](../../../../electron-spin.md) states for each band; any additional valley multiplicity must instead be absorbed into the masses or explicit degeneracy factors.

Let the [conduction band](../../../../conduction-band.md) edge be $E_c$, the [valence band](../../../../valence-band.md) edge $E_v$, and $E_g=E_c-E_v$. The spin-summed conduction [density of states](../../../../density-of-states.md) per [volume](../../../../volume.md) is

$$
g_c(E)=\frac1{2\pi^2}\left(\frac{2m_e^*}{\hbar^2}\right)^{3/2}\sqrt{E-E_c},\qquad E\geq E_c.
$$

Using the nondegenerate limit of the [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md) and the substitution $x=(E-E_c)/(k_BT)$ gives

$$
n=\int_{E_c}^\infty g_c(E)e^{-(E-\mu)/(k_BT)}dE
=N_c e^{-(E_c-\mu)/(k_BT)},
\quad N_c=2\left(\frac{m_e^*k_BT}{2\pi\hbar^2}\right)^{3/2}.
$$

The factor $\sqrt\pi/2$ in the supplied integral produces the normalization. Counting missing [valence band](../../../../valence-band.md) [electrons](../../../../electron.md) similarly gives

$$
p=N_v e^{-(\mu-E_v)/(k_BT)},\qquad
N_v=2\left(\frac{m_h^*k_BT}{2\pi\hbar^2}\right)^{3/2}.
$$

Multiplication cancels the [chemical potential](../../../../chemical-potential-split.md), establishing the [semiconductor mass-action law](../../../../semiconductor-mass-action-law.md):

$$
\boxed{np=N_cN_v e^{-E_g/(k_BT)}
=4\left(\frac{k_BT}{2\pi\hbar^2}\right)^3(m_e^*m_h^*)^{3/2}e^{-E_g/(k_BT)}.}
$$

The result does not require an [intrinsic semiconductor](../../../../intrinsic-semiconductor.md): [semiconductor doping](../../../../semiconductor-doping.md) changes $n$ and $p$ separately while preserving this product under the stated equilibrium and nondegeneracy assumptions.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

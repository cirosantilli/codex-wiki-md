<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\beta=1/(k_BT)$, with $k_B$ the [Boltzmann constant](../../../../boltzmann-constant.md), $T$ the absolute [temperature](../../../../temperature-split.md), and $\mu$ the common equilibrium [chemical potential](../../../../chemical-potential-split.md). The [conduction band](../../../../conduction-band.md) minimum and [valence band](../../../../valence-band.md) maximum are $\epsilon_c$ and $\epsilon_v$; their separation is the [band gap](../../../../band-gap.md) $E_g=\epsilon_c-\epsilon_v$. The positive parameters $m_e,m_h$ in the supplied [density of states](../../../../density-of-states.md) functions are the [band effective masses](../../../../band-effective-mass.md) of [electrons](../../../../electron.md) and [electron holes](../../../../electron-hole.md), not necessarily the bare [electron mass](../../../../electron-mass.md).

The [electron](../../../../electron.md) occupation is the [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md) $f(\epsilon)=[e^{\beta(\epsilon-\mu)}+1]^{-1}$. The appropriate statistical factors are $f_c=f$ for [electrons](../../../../electron.md) and $f_v=1-f$ for [electron holes](../../../../electron-hole.md). In a [nondegenerate semiconductor](../../../../nondegenerate-semiconductor.md), $\epsilon_c-\mu\gg k_BT$ and $\mu-\epsilon_v\gg k_BT$, so the [Boltzmann approximation](../../../../boltzmann-approximation.md) gives

$$
f_c(\epsilon)\simeq e^{-\beta(\epsilon-\mu)},\qquad
f_v(\epsilon)\simeq e^{\beta(\epsilon-\mu)}.
$$

For the [conduction band](../../../../conduction-band.md), set $u=\epsilon-\epsilon_c$ and then $\xi=\beta u$. The supplied integral yields

$$
\begin{aligned}
n&=\frac{(2m_e)^{3/2}}{2\pi^2\hbar^3}
 e^{-\beta(\epsilon_c-\mu)}\int_0^\infty u^{1/2}e^{-\beta u}\,du\\
&=2\left(\frac{m_e}{2\pi\beta\hbar^2}\right)^{3/2}
 e^{-\beta(\epsilon_c-\mu)}=N_c e^{-\beta(\epsilon_c-\mu)}.
\end{aligned}
$$

For the [valence band](../../../../valence-band.md), set $u=\epsilon_v-\epsilon$ to obtain

$$
p=N_v e^{-\beta(\mu-\epsilon_v)},\qquad
N_v=2\left(\frac{m_h}{2\pi\beta\hbar^2}\right)^{3/2}.
$$

The [effective density of states](../../../../effective-density-of-states.md) factors $N_c,N_v$ include the two [spin](../../../../spin.md) states already present in the supplied [density of states](../../../../density-of-states.md) functions. Multiplication cancels the [chemical potential](../../../../chemical-potential-split.md) and gives the [semiconductor mass-action law](../../../../semiconductor-mass-action-law.md)

$$
\boxed{np=N_cN_v e^{-\beta E_g}
=4\left(\frac{\sqrt{m_em_h}\,k_BT}{2\pi\hbar^2}\right)^3
 e^{-E_g/(k_BT)}=n_i^2.}
$$

Here $n_i=\sqrt{N_cN_v}e^{-E_g/(2k_BT)}$ is the [intrinsic carrier concentration](../../../../intrinsic-carrier-concentration.md). Equality $n=p=n_i$ additionally requires an electrically neutral [intrinsic semiconductor](../../../../intrinsic-semiconductor.md). The product law also applies to an equilibrium doped [semiconductor](../../../../semiconductor-split.md) while both populations remain nondegenerate. The derivation assumes parabolic [energy bands](../../../../energy-band.md), the stated [spin degeneracy](../../../../spin-degeneracy.md), and a single common [chemical potential](../../../../chemical-potential-split.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

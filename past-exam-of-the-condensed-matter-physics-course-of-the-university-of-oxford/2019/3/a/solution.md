<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Boltzmann carrier density of a two-dimensional parabolic band](../../../../boltzmann-carrier-density-of-a-two-dimensional-parabolic-band.md) can be derived directly. Use one isotropic parabolic [conduction band](../../../../conduction-band.md), $E(\mathbf k)=E_c+\hbar^2k^2/(2m_e^*)$, with two spin states per [wave vector](../../../../wavevector.md). In the nondegenerate limit the [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md) reduces to its Boltzmann factor. The number per area is therefore

$$
\begin{aligned}
n&=2\int\frac{d^2k}{(2\pi)^2}\exp\left[-\beta\left(E_c-\mu+\frac{\hbar^2k^2}{2m_e^*}\right)\right]\\
&=\frac{e^{-\beta(E_c-\mu)}}\pi\int_0^\infty k\,e^{-\beta\hbar^2k^2/(2m_e^*)}\,dk\\
&=\frac{m_e^*k_BT}{\pi\hbar^2}e^{-\beta(E_c-\mu)}.
\end{aligned}
$$

The integral uses $\int_0^\infty ke^{-ak^2}dk=1/(2a)$. Thus

$$
\boxed{C=\frac{k_B}{\pi\hbar^2},\qquad a=1,\qquad b=1.}
$$

Equivalently, the two-dimensional [density of states](../../../../density-of-states.md) is constant, $D_c=m_e^*/(\pi\hbar^2)$, and $n=N_c e^{-\beta(E_c-\mu)}$ with $N_c=D_ck_BT$. These expressions include twofold [spin degeneracy](../../../../spin-degeneracy.md) and one valley. With a general total band degeneracy $g_c$, replace the factor $1/\pi$ by $g_c/(2\pi)$; extra valleys or occupied confinement subbands would change the coefficient.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

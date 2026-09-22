<h1 id="section-b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the nondegenerate [conduction band](../../../../../conduction-band.md), the [Fermi-Dirac distribution](../../../../../fermi-dirac-distribution.md) reduces to its [Boltzmann distribution](../../../../../boltzmann-distribution.md) tail. Thus

$$
\begin{aligned}
n&=\int_{\epsilon_c}^\infty g_e(\epsilon)e^{-(\epsilon-\mu)/(k_BT)}d\epsilon\\
&=N_c e^{-(\epsilon_c-\mu)/(k_BT)},\qquad
\boxed{N_c=2\left(\frac{m_e^*k_BT}{2\pi\hbar^2}\right)^{3/2}}.
\end{aligned}
$$

Here the substitution $x=(\epsilon-\epsilon_c)/(k_BT)$ leaves $\int_0^\infty x^{1/2}e^{-x}dx=\sqrt\pi/2$. For [electron holes](../../../../../electron-hole.md) use the empty-state probability $1-f(\epsilon)\simeq e^{(\epsilon-\mu)/(k_BT)}$, not the conduction-band Boltzmann factor. This gives

$$
p=N_v e^{-(\mu-\epsilon_v)/(k_BT)},\qquad
\boxed{N_v=2\left(\frac{m_h^*k_BT}{2\pi\hbar^2}\right)^{3/2}}.
$$

The [chemical potential](../../../../../chemical-potential-split.md) cancels in the product. With $E_g=\epsilon_c-\epsilon_v$,

$$
\boxed{np=N_cN_v e^{-E_g/(k_BT)}
=\frac12(m_e^*m_h^*)^{3/2}\left(\frac{k_BT}{\pi\hbar^2}\right)^3e^{-E_g/(k_BT)}=n_i^2.}
$$

This [semiconductor mass-action law](../../../../../semiconductor-mass-action-law.md) holds in thermal equilibrium for nondegenerate carriers, including a doped [semiconductor](../../../../../semiconductor-split.md). Only in an [intrinsic semiconductor](../../../../../intrinsic-semiconductor.md) must $n=p=n_i$. The factors $N_c,N_v$ are the [effective density of states](../../../../../effective-density-of-states.md); the factor $1/2$ in the final expression follows from the two spin factors already included in (a).

## ↑ Ancestors (14)

1. [B](../b.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the quantum condensed matter course of the University of Cambridge](../../../../split.md)
6. [Quantum Condensed Matter course of the University of Cambridge](../../../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)

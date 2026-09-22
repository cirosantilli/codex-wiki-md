<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume uncompensated [donor impurities](../../../../../donor-impurity.md), negligible intrinsic [electron holes](../../../../../electron-hole.md), and a nondegenerate [conduction band](../../../../../conduction-band.md). Then [charge neutrality](../../../../../charge-neutrality.md) equates the conduction [electron number density](../../../../../electron-number-density.md) to the ionized-donor [number density](../../../../../number-density.md):

$$
n=n_{\rm empty},\qquad n_{\rm full}=N_D-n.
$$

The low-[temperature](../../../../../temperature-split.md) condition relative to the [band gap](../../../../../band-gap.md) supports neglect of intrinsic carriers; one also needs $n_i\ll n$ and the [Boltzmann approximation](../../../../../boltzmann-approximation.md) for the conduction [electrons](../../../../../electron.md). Combining part (b)(i) with the [effective density of states](../../../../../effective-density-of-states.md) result gives

$$
\frac{N_D-n}{n}=e^{\beta(\mu-\epsilon_D)},\qquad
n=N_c e^{\beta(\mu-\epsilon_c)}.
$$

Eliminate the [chemical potential](../../../../../chemical-potential-split.md) by writing $e^{\beta(\mu-\epsilon_D)}=(n/N_c)e^{\beta(\epsilon_c-\epsilon_D)}$. With the donor binding [energy](../../../../../energy-split.md) $E_i=\epsilon_c-\epsilon_D>0$,

$$
\boxed{\frac{n^2}{N_D-n}=N_c e^{-\beta E_i}
=2\left(\frac{m_e}{2\pi\beta\hbar^2}\right)^{3/2}e^{-\beta E_i}.}
$$

Writing $A(T)=N_c e^{-\beta E_i}$, the physical root of the resulting [quadratic equation](../../../../../quadratic-equation.md) is

$$
n=\frac{\sqrt{A^2+4AN_D}-A}{2}.
$$

This lies between zero and $N_D$. At [semiconductor carrier freeze-out](../../../../../semiconductor-carrier-freeze-out.md), $A\ll N_D$, it becomes $n\simeq\sqrt{N_DN_c}\,e^{-E_i/(2k_BT)}$; at essentially complete ionization, $A\gg N_D$, it tends to $N_D$. Including [donor charge-state degeneracy](../../../../../donor-charge-state-degeneracy.md) would replace $A$ by $A\,g_{\rm empty}/g_{\rm full}$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the condensed matter physics course of the University of Oxford](../../../../split.md)
6. [Condensed matter physics course of the University of Oxford](../../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
7. [Year 3 of the physics course of the University of Oxford](../../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

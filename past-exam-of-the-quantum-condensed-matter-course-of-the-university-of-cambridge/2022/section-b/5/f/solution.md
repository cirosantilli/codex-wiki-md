<h1 id="section-b/5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Let the common uncoupled [Fermi wavevector](../../../../../fermi-wavevector.md) be $k_0$. Equal [carrier densities](../../../../../carrier-density.md) imply equal [Fermi surface](../../../../../fermi-surface.md) volumes, and hence equal radii for the spherical spin-degenerate electron pockets. The conserved total density is

$$
n_{\rm tot}=\frac{2k_0^3}{3\pi^2}.
$$

If hybridisation leaves only one occupied electron-like band, state counting gives

$$
\boxed{k_F=2^{1/3}k_0,\qquad p_F=2^{1/3}p_0,\qquad
\frac{\Delta p_F}{p_0}=2^{1/3}-1\simeq0.260.}
$$

This is the familiar single-large-Fermi-surface answer. It requires the other hybridised band to be empty.

**For finite heavy-band mass, that conclusion does not follow from an arbitrary nonzero coupling.** At sufficiently small $\alpha$, the upper band still has an occupied pocket, so there are two Fermi momenta, not one. The exact fixed-density statement is [Fermi-volume conservation in two hybridized electron bands](../../../../../fermi-volume-conservation-in-two-hybridized-electron-bands.md):

$$
\boxed{k_{F,-}^3+k_{F,+}^3=2k_0^3.}
$$

For an explicit weak-coupling check, write $E_p=Ak^2$, $E_h=C+Bk^2$, with $0<B\ll A$, and enforce the uncoupled equality at $k_0$: $C=(A-B)k_0^2$, $\mu_0=Ak_0^2$. Put $\mu=\mu_0+\delta\mu$ and $y=k_F^2-k_0^2$. The Fermi-surface equation is

$$
(\delta\mu-Ay)(\delta\mu-By)-\alpha^2=0.
$$

At fixed density $\delta\mu=O(\alpha^2)$, giving

$$
\boxed{k_{F,\mp}=k_0\pm\frac{\alpha}{2k_0\sqrt{AB}}+O(\alpha^2).}
$$

For arbitrary coupling, put $q_\pm=k_{F,\mp}^2$. The roots of the same [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md), before discarding unoccupied pockets, are

$$
q_\pm=\frac{(A+B)\mu-AC\pm\sqrt{[(A-B)\mu-AC]^2+4AB\alpha^2}}{2AB}.
$$

Choose the [chemical potential](../../../../../chemical-potential-split.md) so that $[\max(q_+,0)]^{3/2}+[\max(q_-,0)]^{3/2}=2k_0^3$. This specifies the [Fermi momentum](../../../../../fermi-momentum.md) of each pocket for any supplied curvatures and coupling.

The transition to one occupied pocket occurs at $\mu=E_+(0)$. Set $q_*=2^{2/3}k_0^2$; at the transition the two squared radii are $q_*$ and zero. Their sum and product give

$$
\mu_c=\frac{A(C+Bq_*)}{A+B},\qquad
\boxed{\alpha_c^2=\mu_c(\mu_c-C)
=\frac{AB(C+Bq_*)(Aq_*-C)}{(A+B)^2}.}
$$

For $0<\alpha<\alpha_c$ there are two pockets; for $\alpha\geq\alpha_c$ the only nonzero radius is $2^{1/3}k_0$. The outer radius grows continuously and the inner one shrinks. The nearly [flat band](../../../../../flat-band.md) limit can make depopulation occur at a small coupling, but the mass ratio or a single-surface assumption is needed to turn the question into a unique finite-coupling numerical change.

## ↑ Ancestors (14)

1. [F](../f.md)
2. [5](../../5.md)
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

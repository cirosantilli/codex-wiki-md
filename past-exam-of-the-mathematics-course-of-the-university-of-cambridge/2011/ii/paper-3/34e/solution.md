<h1 id="34e/solution">Solution</h1>

↑ **Parent:** [34E](../34e.md)

[Bloch theorem](../../../../../bloch-s-theorem.md) states that energy eigenfunctions in a [Bravais lattice](../../../../../bravais-lattice.md) potential may be chosen as

$$
\boxed{\psi_{n\mathbf k}(\mathbf r)=e^{i\mathbf k\cdot\mathbf r}u_{n\mathbf k}(\mathbf r),\qquad u_{n\mathbf k}(\mathbf r+\mathbf l)=u_{n\mathbf k}(\mathbf r).}
$$

The wavevector is defined modulo a [reciprocal lattice](../../../../../reciprocal-lattice.md) vector, so one can restrict it to the first [Brillouin zone](../../../../../brillouin-zone.md). This follows because lattice translations commute with the Hamiltonian and have simultaneous eigenvalues $e^{i\mathbf k\cdot\mathbf l}$.

In one dimension write $V(x)=\sum_GV_Ge^{iGx}$ with $G=2\pi j/a$ and expand a Bloch state as $\psi_k=\sum_Gc_Ge^{i(k+G)x}$. The [Schrödinger equation](../../../../../schrodinger-equation.md) becomes

$$
\left[\frac{\hbar^2(k+G)^2}{2m}-E\right]c_G+\sum_{G'}V_{G-G'}c_{G'}=0.
$$

For zero potential, the parabolas $E_G^0(k)=\hbar^2(k+G)^2/(2m)$ fold into the Brillouin zone. A weak potential shifts a nondegenerate level by $V_0$ at first order, with second-order correction $\sum_{G\ne0}|V_G|^2/(E_0^0-E_G^0)$ where the denominators stay away from zero. This expansion fails near crossings, where [degenerate perturbation theory](../../../../../degenerate-perturbation-theory.md) is required.

At the first zone boundary, put $G=2\pi/a$ and $k=G/2+q$. The nearly degenerate waves with momenta $\hbar k$ and $\hbar(k-G)$ are coupled by $V_G$. Retaining their two-dimensional subspace gives

$$
H_{\rm eff}=\begin{pmatrix}\epsilon_k+V_0&V_G\\V_G^*&\epsilon_{k-G}+V_0\end{pmatrix},\quad\epsilon_p=\frac{\hbar^2p^2}{2m}.
$$

Diagonalizing produces

$$
\boxed{E_\pm(q)=V_0+\frac{\hbar^2}{2m}\left(\frac{G^2}{4}+q^2\right)\pm\sqrt{\left(\frac{\hbar^2Gq}{2m}\right)^2+|V_G|^2}.}
$$

At $q=0$ there is a gap $\boxed{\Delta E=2|V_G|}$: the two standing-wave combinations sample the periodic potential differently. Similar Bragg degeneracies occur at $k=j\pi/a$, with gaps controlled to first order by the corresponding Fourier components. If that component vanishes, a gap need not open at first order. Between the gaps the continuous energy eigenvalues form [energy bands](../../../../../energy-band.md), periodically represented in the reduced-zone scheme. For the first zone edge, the curvature of the upper and lower branches gives a minimum and a maximum respectively for a sufficiently weak nonzero potential, so the avoided crossing is a genuine local forbidden energy interval.

At zero temperature electrons occupy states up to the [Fermi energy](../../../../../fermi-energy.md). The [Fermi surface](../../../../../fermi-surface.md) is the set $E_n(\mathbf k)=E_F$ separating occupied from unoccupied states within partially filled bands (Fermi points in one dimension). A partially filled band supplies arbitrarily nearby empty states, allowing occupations to respond to a weak electric field and conduct. Completely filled bands give no net current from such a redistribution; if the next empty band is separated by a positive [band gap](../../../../../band-gap.md), the system is a band insulator. Band overlap can instead yield a metal even at an integer band filling. At finite temperature an insulator can conduct through thermally excited electrons and holes.

## ↑ Ancestors (10)

1. [34E](../34e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

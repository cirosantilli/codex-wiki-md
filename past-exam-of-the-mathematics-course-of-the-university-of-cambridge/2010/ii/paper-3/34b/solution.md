<h1 id="34b/solution">Solution</h1>

↑ **Parent:** [34B](../34b.md)

The [Bloch theorem](../../../../../bloch-s-theorem.md) says that for a translation-invariant lattice [Hamiltonian](../../../../../hamiltonian.md), eigenstates can be chosen as $\psi_k(x+a)=e^{ika}\psi_k(x)$, or $\psi_k(x)=e^{ikx}u_k(x)$ with $u_k$ periodic of period $a$. The localized site orbitals are translates, $\phi_n(x)=\phi_0(x-na)$ and $\chi_n(x)=\chi_0(x-na)$. In the [tight-binding model](../../../../../tight-binding.md), neglect intersite overlap and use

$$
\psi(x,t)=\sum_n\bigl(b_n(t)\phi_n(x)+c_n(t)\chi_n(x)\bigr).
$$

Projecting the [Schrödinger equation](../../../../../schrodinger-equation.md) onto each localized orbital gives its onsite energy times its own coefficient, plus the four stated neighbor matrix elements. Thus

$$
\boxed{\begin{aligned}
i\hbar\dot b_n&=E_0b_n-A(b_{n-1}+b_{n+1}+c_{n-1}+c_{n+1}),\\
i\hbar\dot c_n&=E_1c_n-A(c_{n-1}+c_{n+1}+b_{n-1}+b_{n+1}).
\end{aligned}}
$$

For the Bloch amplitudes, set $z=\cos ka$. The coefficient eigenproblem is

$$
\begin{pmatrix}E_0-2Az&-2Az\\-2Az&E_1-2Az\end{pmatrix}\binom BC=E\binom BC,
$$

so the two [energy bands](../../../../../energy-band.md) are

$$
\boxed{E_\pm(k)=\frac{E_0+E_1}{2}-2A\cos ka
\pm\frac12\sqrt{(E_1-E_0)^2+16A^2\cos^2ka}.}
$$

A first [Brillouin zone](../../../../../brillouin-zone.md) is $-\pi/a\le k<\pi/a$; wavevectors differing by $2\pi/a$ are equivalent. Put $\Sigma=E_0+E_1$, $D=\sqrt{(E_1-E_0)^2+16A^2}$. Each band is nonincreasing as a function of $z\in[-1,1]$, because $dE_\pm/dz=-2A\pm8A^2z/\sqrt{(E_1-E_0)^2+16A^2z^2}\le0$. Hence

$$
\boxed{E_{\pm,\min}=\Sigma/2-2A\pm D/2,\qquad
E_{\pm,\max}=\Sigma/2+2A\pm D/2,\qquad
\Delta E=E_{+,\min}-E_{-,\max}=D-4A.}
$$

The extrema occur at $k=0$ and at the zone edge; they may be nonunique when $E_0=E_1$, in which case the gap vanishes. In the trial wavefunction, replacing $x$ by $x+a$ and reindexing $n$ produces exactly the factor $e^{ika}$, verifying [Bloch theorem](../../../../../bloch-s-theorem.md) directly.

An [electrical conductor](../../../../../electrical-conductor.md) has available nearby unoccupied states in a partially filled band or overlapping bands. A [band insulator](../../../../../band-insulator.md) has filled lower bands separated from empty higher bands by a large gap. A [semiconductor](../../../../../semiconductor.md) has the same filled-band structure with a smaller gap, so thermal excitation or doping supplies mobile electrons and holes. Band filling and carrier availability, not just the existence of two bands, determine which description applies.

## ↑ Ancestors (10)

1. [34B](../34b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

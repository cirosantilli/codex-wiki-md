<h1 id="section-b/b4/solution">Solution</h1>

↑ **Parent:** [B4](../b4.md)

For physical [spin ladder operators](../../../../spin-ladder-operator.md), $S_j^\pm=S_j^x\pm iS_j^y$. Operators at distinct sites commute. Expanding the two products cancels their cross terms and gives

$$
\frac12(S_j^+S_{j+1}^-+S_j^-S_{j+1}^+)=S_j^xS_{j+1}^x+S_j^yS_{j+1}^y.
$$

Adding the remaining component proves

$$
\boxed{\mathbf S_j\cdot\mathbf S_{j+1}=\frac12(S_j^+S_{j+1}^-+S_j^-S_{j+1}^+)+S_j^zS_{j+1}^z.}
$$

For [spin one-half](../../../../spin-one-half.md), $S^+|\downarrow\rangle=\hbar|\uparrow\rangle$, $S^-|\uparrow\rangle=\hbar|\downarrow\rangle$, and raising an up [spin](../../../../spin.md) or lowering a down [spin](../../../../spin.md) gives zero. These formulas restore the physical $\hbar$ factors implicit in the dimensionless ladder hint.

Let $|n\rangle$ abbreviate the state with the only down [spin](../../../../spin.md) at site $n$, keeping $|\psi_0\rangle$ for the fully up state. If $n$ lies on neither end of bond $(j,j+1)$, that bond contains two up [spins](../../../../spin.md). The ladder terms vanish, while $S_j^zS_{j+1}^z$ gives $\hbar^2/4$. Thus

$$
\mathbf S_j\cdot\mathbf S_{j+1}|n\rangle=\frac{\hbar^2}{4}|n\rangle\qquad(n\ne j,j+1).
$$

For a down [spin](../../../../spin.md) at $j$, the $z$ product is instead $-\hbar^2/4$, and $S_j^+S_{j+1}^-$ moves it to $j+1$ with [amplitude](../../../../wave-amplitude.md) $\hbar^2$. For a down [spin](../../../../spin.md) at $j+1$, the other ladder product moves it back. Therefore

$$
\boxed{\mathbf S_j\cdot\mathbf S_{j+1}|j\rangle=\frac{\hbar^2}{4}(2|j+1\rangle-|j\rangle),\qquad \mathbf S_j\cdot\mathbf S_{j+1}|j+1\rangle=\frac{\hbar^2}{4}(2|j\rangle-|j+1\rangle).}
$$

Every bond in $|\psi_0\rangle$ is aligned, so summing its $N$ bond energies gives

$$
\boxed{H|\psi_0\rangle=E_0|\psi_0\rangle,\qquad E_0=-\frac{NJ}{4}.}
$$

This is indeed a [ground-state energy](../../../../ground-state-energy.md): a pair of spin-one-half particles has $\mathbf S_j\cdot\mathbf S_{j+1}$ [eigenvalues](../../../../eigenvalue.md) $\hbar^2/4$ and $-3\hbar^2/4$, so each ferromagnetic bond is bounded below by $-J/4$, simultaneously attained by the fully aligned state. The isotropic [Heisenberg model](../../../../heisenberg-model.md) has a whole maximum-total-spin ground multiplet, not a unique all-up [ground state](../../../../ground-state.md).

In the [single-excitation subspace](../../../../single-excitation-subspace.md), only the two bonds adjacent to the down [spin](../../../../spin.md) differ from the aligned background. Their diagonal [energy](../../../../energy-split.md) increase is $J$, and each neighboring hop has [amplitude](../../../../wave-amplitude.md) $-J/2$. Hence, with periodic site indices,

$$
\boxed{H|n\rangle=(E_0+J)|n\rangle-\frac J2(|n-1\rangle+|n+1\rangle).}
$$

This is an exact finite-dimensional hopping problem. Choose the active one-site translation convention $T|n\rangle=|n+1\rangle$. A periodic plane-wave coefficient pattern requires $e^{iq(n+N)a}=e^{iqna}$, so

$$
\boxed{q=\frac{2\pi\ell}{Na},\qquad \ell\in\mathbb Z,\qquad q\ \text{identified modulo }\frac{2\pi}{a}.}
$$

There are $N$ independent such [wavevectors](../../../../wavevector.md), for example one set of $N$ consecutive integers $\ell$ in a [Brillouin zone](../../../../brillouin-zone.md). The normalized [one-magnon Bloch states on a ring](../../../../one-magnon-bloch-states-on-a-ring.md) are $|q\rangle=N^{-1/2}\sum_{n=1}^Ne^{iqna}|n\rangle$. Reindexing with the periodic coefficient condition gives $T|q\rangle=e^{-iqa}|q\rangle$ and hence $T^N|q\rangle=|q\rangle$.

There is a logical qualification to the condition stated in the paper. On an $N$-site ring $T^N=I$ already holds for every state. In particular, the finite sum written with an arbitrary real $q$ also returns to itself after $N$ translations; that condition alone does not quantize $q$. The displayed allowed values are the ones for which the ansatz is a single one-site translation [eigenstate](../../../../eigenstate.md), equivalently a consistently periodic [plane wave](../../../../plane-wave.md). This is the additional condition needed for the subsequent energy-eigenstate argument. Other $q$ values generally describe superpositions of the allowed [momentum](../../../../momentum-split.md) modes.

Apply the hopping [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) and shift the summation index using [periodic boundary condition](../../../../periodic-boundary-conditions.md). The coefficients from $|n-1\rangle$ and $|n+1\rangle$ are respectively $e^{iqa}$ and $e^{-iqa}$ times the original coefficient. Thus

$$
H|q\rangle=\left(E_0+J-\frac J2e^{iqa}-\frac J2e^{-iqa}\right)|q\rangle,
$$

and the [nearest-neighbour ferromagnetic magnon dispersion](../../../../nearest-neighbour-ferromagnetic-magnon-dispersion.md) is

$$
\boxed{E(q)=E_0+J[1-\cos(qa)]=E_0+2J\sin^2\frac{qa}{2}.}
$$

The unnormalized state in the question has the same [energy](../../../../energy-split.md). Distinct allowed [momenta](../../../../momentum-split.md) are [orthogonal](../../../../orthogonal-vectors.md), since $N^{-1}\sum_ne^{i(q-q')na}=\delta_{qq'}$ over one set of representatives.

<a id="section-b/b4/image-exact-one-magnon-dispersion-and-its-discrete-ring-momenta-over-two-reciprocal-periods"></a>
![](../../../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2018-magnon-dispersion.png)

**[Figure 4](#section-b/b4/image-exact-one-magnon-dispersion-and-its-discrete-ring-momenta-over-two-reciprocal-periods). Exact one-magnon dispersion and its discrete ring momenta over two reciprocal periods**.

For large $N$ the sampled [wavevectors](../../../../wavevector.md) become dense, and the requested sketch is the periodic curve $[E(q)-E_0]/J=1-\cos(qa)$ over $-2\pi<qa<2\pi$. It has a zero at $q=0$ and tends to the equivalent zero at either open endpoint; maxima $2J$ occur at $q=\pm\pi/a$. Near any equivalent zero,

$$
\boxed{E(q)-E_0=\frac{Ja^2q^2}{2}+O(q^4),}
$$

using $q$ measured from that zero. The low-momentum [ferromagnetic magnon](../../../../ferromagnetic-magnon.md) is quadratic, with [group velocity](../../../../group-velocity.md) $\hbar^{-1}dE/dq=(Ja/\hbar)\sin(qa)$. The $q=0$ state is proportional to the total [spin lowering operator](../../../../spin-lowering-operator.md) acting on $|\psi_0\rangle$, so it belongs to the same ground multiplet and has exactly zero excitation [energy](../../../../energy-split.md). Extending the plot beyond one reciprocal period repeats states rather than adding new independent modes. The lattice spacing $a$ is the nearest-neighbor chord length specified in the paper; $Na$ is the translation length in this lattice description, not necessarily the continuous circumference of a circular arrangement.

## ↑ Ancestors (13)

1. [B4](../b4.md)
2. [Section B](../../section-b.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)

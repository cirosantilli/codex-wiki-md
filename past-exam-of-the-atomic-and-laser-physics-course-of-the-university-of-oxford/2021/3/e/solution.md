<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

To derive [fermionic Einstein-coefficient relations](../../../../fermionic-einstein-coefficient-relations.md), first consider an idealized emitter that can exchange one ultrarelativistic [fermion](../../../../fermion.md) with the bath, with zero [chemical potential](../../../../chemical-potential-split.md). Let $\mathcal D_\nu=d\,4\pi\nu^2/c^3$ be its [density of states](../../../../density-of-states.md) per volume and ordinary [frequency](../../../../frequency.md), with $d$ populated helicity states; for one [neutrino](../../../../neutrino.md) helicity $d=1$, whereas the corresponding [photon](../../../../photon.md) count is two. The [Fermi-Dirac distribution](../../../../fermi-dirac-distribution.md) gives

$$
f_\nu=\frac1{e^{h\nu/(k_BT)}+1},\qquad u_\nu=h\nu\mathcal D_\nu f_\nu.
$$

[Pauli blocking](../../../../pauli-blocking.md) changes the final-state factor in downward emission from the bosonic $1+f$ to $1-f$. Define positive coefficients $B_{12},C_{21}$ and $A_{21}=C_{21}h\nu\mathcal D_\nu$. The upward rate per lower emitter is $B_{12}u_\nu$, and the downward rate per upper emitter is

$$
A_{21}(1-f_\nu)=A_{21}-C_{21}u_\nu.
$$

Thermal [detailed balance](../../../../detailed-balance.md), $n_1B_{12}u_\nu=n_2(A_{21}-C_{21}u_\nu)$ with $n_2/n_1=(g_2/g_1)e^{-h\nu/(k_BT)}$, yields

$$
\boxed{g_1B_{12}=g_2C_{21},\qquad
\frac{A_{21}}{C_{21}}=d\,\frac{4\pi h\nu^3}{c^3}.}
$$

For example, substituting $e^{h\nu/(k_BT)}=x$ reduces the balance equation to $B_{12}=(g_2/g_1)C_{21}$ because $x f_\nu=1-f_\nu$.

If one insists on the original additive notation $A_{21}+B_{21}u_\nu$, its formal coefficient is negative:

$$
\boxed{B_{21}=-C_{21},\qquad g_1B_{12}=-g_2B_{21},\qquad
A_{21}/B_{21}=-d\,4\pi h\nu^3/c^3.}
$$

A negative correction means inhibited emission into occupied modes, not a negative total decay rate; $0\leq f_\nu\leq1$ ensures positivity. The dimensions are those of part (a), and the factor of two relative to the [photon](../../../../photon.md) density is a helicity count, independent of the statistical sign.

There is a physical qualification: ordinary electronic [energy levels](../../../../energy-level.md) of the same [chemical atom](../../../../atom-physics.md) have the same [fermion parity](../../../../fermion-parity.md), and cannot interconvert by emission or absorption of a single [neutrino](../../../../neutrino.md). A realizable single-[fermion](../../../../fermion.md) emitter must change the relevant particle-number and parity sector, with matching [conservation laws](../../../../conservation-law.md). For ordinary atomic levels, neutrino-pair processes would require a different calculation. A bath with nonzero [chemical potential](../../../../chemical-potential-split.md) would also require the corresponding chemical-equilibrium population ratio. The calculation above is the intended single-mode statistical analogy under explicit assumptions.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

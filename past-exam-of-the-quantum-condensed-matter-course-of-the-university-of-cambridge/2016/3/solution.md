<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**[mass](../../../mass.md) as [band curvature](../../../band-curvature.md).** In a periodic potential, a weakly forced [electron](../../../electron.md) is usefully described by a [wave packet](../../../wave-packet.md) confined to one [energy band](../../../energy-band.md). Its [group velocity](../../../group-velocity.md) is

$$
v_i=\frac1\hbar\frac{\partial\varepsilon_n}{\partial k_i},\qquad \hbar\dot k_j=F_j.
$$

Differentiating the [velocity](../../../velocity.md) gives

$$
\dot v_i=\sum_j(m^{*-1})_{ij}F_j,\qquad \boxed{(m^{*-1})_{ij}=\frac1{\hbar^2}\frac{\partial^2\varepsilon_n}{\partial k_i\partial k_j}.}
$$

This [effective-mass tensor](../../../effective-mass-tensor.md) describes the band response, not a change of the [electron](../../../electron.md)'s bare [rest mass](../../../invariant-mass.md). Along a principal direction, a steep upward curvature gives a small positive [mass](../../../mass.md) and a flatter curvature a larger one. Near a band maximum the [electron](../../../electron.md) curvature and [effective mass](../../../band-effective-mass.md) are negative; the corresponding missing-electron description uses positive [electron hole](../../../electron-hole.md) masses. Anisotropy produces distinct principal masses, and strong nonparabolicity makes them [momentum](../../../momentum-split.md) dependent. The single-band semiclassical description assumes fields weak and slowly varying enough to avoid substantial interband transitions.

**[Lattice](../../../lattice.md) [symmetry](../../../symmetry-physics.md) and [Bloch's theorem](../../../bloch-s-theorem-split.md).** Use the active [spatial translation operator](../../../spatial-translation-operator.md) $T_{\mathbf a}\psi(\mathbf r)=\psi(\mathbf r-\mathbf a)$. A lattice-periodic [scalar](../../../scalar.md) potential satisfies $V(\mathbf r+\mathbf a)=V(\mathbf r)$, while the kinetic term is translation invariant. Therefore $[H,T_{\mathbf a}]=0$. The [lattice](../../../lattice.md) translations also commute with one another, so they can be diagonalized simultaneously with $H$, including within a degenerate [energy](../../../energy-split.md) subspace.

For a common [eigenstate](../../../eigenstate.md), write $T_{\mathbf a}\psi=t(\mathbf a)\psi$. [Unitarity](../../../unitary-operator.md) gives $|t(\mathbf a)|=1$, and the group law gives $t(\mathbf a+\mathbf b)=t(\mathbf a)t(\mathbf b)$. On primitive Bravais vectors $\mathbf a_j$, choose $t(\mathbf a_j)=e^{-i\mathbf k\cdot\mathbf a_j}$. Every [lattice](../../../lattice.md) vector is an integer combination of these generators, hence

$$
T_{\mathbf a}\psi_{n\mathbf k}=e^{-i\mathbf k\cdot\mathbf a}\psi_{n\mathbf k},\qquad \psi_{n\mathbf k}(\mathbf r+\mathbf a)=e^{i\mathbf k\cdot\mathbf a}\psi_{n\mathbf k}(\mathbf r).
$$

The vector $\mathbf k$ is defined modulo a [reciprocal lattice](../../../reciprocal-lattice.md) vector. The band index labels the different [energy](../../../energy-split.md) eigenstates with the same translation character. Define $u_{n\mathbf k}(\mathbf r)=e^{-i\mathbf k\cdot\mathbf r}\psi_{n\mathbf k}(\mathbf r)$. The phase factors cancel under a [lattice translation](../../../lattice-translation.md), proving [Bloch's theorem](../../../bloch-s-theorem-split.md) in its usual form:

$$
\boxed{\psi_{n\mathbf k}(\mathbf r)=e^{i\mathbf k\cdot\mathbf r}u_{n\mathbf k}(\mathbf r),\qquad u_{n\mathbf k}(\mathbf r+\mathbf a)=u_{n\mathbf k}(\mathbf r).}
$$

This is the [Translation-character proof of Bloch theorem](../../../translation-character-proof-of-bloch-theorem.md); the [commutator](../../../commutator.md) guarantees a [basis](../../../basis.md) of such states, even when an arbitrary [superposition](../../../superposition-principle.md) of different translation characters is not itself a translation [eigenstate](../../../eigenstate.md).

**Periodic [Hamiltonian](../../../hamiltonian.md).** Acting once with [momentum](../../../momentum-split.md) gives $\mathbf p(e^{i\mathbf k\cdot\mathbf r}u)=e^{i\mathbf k\cdot\mathbf r}(\mathbf p+\hbar\mathbf k)u$. Applying it again and cancelling the common plane-wave factor yields

$$
\boxed{H(\mathbf k)u_{n\mathbf k}=\left[\frac{(\mathbf p+\hbar\mathbf k)^2}{2m}+V(\mathbf r)\right]u_{n\mathbf k}=\varepsilon_n(\mathbf k)u_{n\mathbf k}.}
$$

The [Bloch Hamiltonian](../../../bloch-hamiltonian.md) acts on lattice-periodic functions in a [unit cell](../../../unit-cell.md). Expanding its square separates a zero-momentum [Hamiltonian](../../../hamiltonian.md), a term linear in $\mathbf k$ and an identity term quadratic in $\mathbf k$.

**Expansion about the zone centre.** Let $|n\rangle=u_{n0}$, $E_n=\varepsilon_n(0)$, and normalize all these states using a unit-cell [inner product](../../../inner-product-split.md). For the real [scalar](../../../scalar.md) [Hamiltonian](../../../hamiltonian.md) in the question, a nondegenerate zone-centre eigenfunction can be chosen real. Then

$$
\langle n|\mathbf p|n\rangle=-\frac{i\hbar}{2}\int_{\rm cell}\nabla(u_{n0}^2)\,d^3r=0,
$$

because opposite unit-cell faces cancel. Equivalently, [time-reversal symmetry](../../../t-symmetry.md) forbids a nonzero [electric current](../../../electric-current.md) in this nondegenerate spinless state. This explains why no linear [energy](../../../energy-split.md) term appears; it should not simply be omitted without a [symmetry](../../../symmetry-physics.md) or extremum argument.

The first-order [energy](../../../energy-split.md) shift is therefore $\hbar^2k^2/(2m)$. In the second-order sum the quadratic term is proportional to the identity and has no off-diagonal [matrix elements](../../../matrix-element.md). Only the linear [momentum](../../../momentum-split.md) vertex contributes. [Second-order nondegenerate perturbation theory](../../../second-order-nondegenerate-perturbation-theory.md) gives the [momentum matrix-element expansion of band energy](../../../momentum-matrix-element-expansion-of-band-energy.md)

$$
\boxed{\varepsilon_n(\mathbf k)=E_n+\frac{\hbar^2k^2}{2m}+\frac{\hbar^2}{m^2}\sum_{l\ne n}\frac{|\langle n|\mathbf k\cdot\mathbf p|l\rangle|^2}{E_n-E_l}+O(|\mathbf k|^4).}
$$

[Hermitian operator](../../../hermitian-operator.md) makes the two reciprocal [matrix elements](../../../matrix-element.md) [complex conjugates](../../../complex-conjugate.md). All other periodic eigenstates at $\mathbf k=0$ enter the sum. The remainder is even because [time-reversal symmetry](../../../t-symmetry.md) gives $\varepsilon_n(\mathbf k)=\varepsilon_n(-\mathbf k)$ near this isolated state. At a degeneracy the denominators signal the need for [degenerate perturbation theory](../../../degenerate-perturbation-theory.md) instead.

**[mass](../../../mass.md) ratio and the printed formula.** Write $p^i_{nl}=\langle n|p_i|l\rangle$. Differentiating the quadratic [energy](../../../energy-split.md) yields

$$
\boxed{(m^{*-1})_{ij}=\frac{\delta_{ij}}m+\frac2{m^2}\sum_{l\ne n}\frac{\operatorname{Re}(p^i_{nl}p^j_{ln})}{E_n-E_l}.}
$$

For a specified unit direction $\mathbf e$, the resulting [scalar](../../../scalar.md) [mass](../../../mass.md) ratio is

$$
\boxed{\frac m{m^*_{\mathbf e}}=1+\frac2m\sum_{l\ne n}\frac{|\langle n|\mathbf e\cdot\mathbf p|l\rangle|^2}{E_n-E_l}.}
$$

In an isotropic three-dimensional band, averaging equivalent directions gives

$$
\boxed{\frac m{m^*}=1+\frac{2}{3m}\sum_{l\ne n}\frac{|\langle n|\mathbf p|l\rangle|^2}{E_n-E_l}.}
$$

Coupling to lower bands contributes positively to inverse [mass](../../../mass.md); coupling to higher bands contributes negatively. Their signs and [matrix elements](../../../matrix-element.md) determine the actual curvature.

The original PDF prints $m^*=\hbar^2[\nabla_{\mathbf k}^2\varepsilon_n]^{-1}$. **Taken literally as a three-dimensional [Laplacian](../../../laplacian.md), this misses a factor of three for an isotropic [scalar](../../../scalar.md) [mass](../../../mass.md).** The correct identities are

$$
\frac{\nabla_{\mathbf k}^2\varepsilon_n}{\hbar^2}=\operatorname{tr}(m^{*-1}),\qquad m^*=\frac{3\hbar^2}{\nabla_{\mathbf k}^2\varepsilon_n}\quad\text{in three isotropic dimensions}.
$$

The printed expression would return $m/3$ even for the free dispersion $\hbar^2k^2/(2m)$. It is correct in one dimension, or if its [second derivative](../../../second-derivative.md) is interpreted directionally. For completeness, its literal three-dimensional trace ratio would instead be $3+(2/m)\sum_{l\ne n}|\langle n|\mathbf p|l\rangle|^2/(E_n-E_l)$; that is the trace of the dimensionless inverse-mass [tensor](../../../tensor.md), not the usual [scalar](../../../scalar.md) $m/m^*$.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [2016](../../2016-split.md)
3. [Past exam of the quantum condensed matter course of the University of Cambridge](../../split.md)
4. [Quantum Condensed Matter course of the University of Cambridge](../../../quantum-condensed-matter-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)

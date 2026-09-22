<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Since every [quasiparticle](../../../../quasiparticle.md) [energy](../../../../energy-split.md) is positive, the [ground state](../../../../ground-state.md) is the vacuum of all the $\alpha_p$ [annihilation operators](../../../../annihilation-operator.md), including $\alpha_0=c_0$. Its zero-momentum mode is therefore empty. For each positive momentum, the inverse [Bogoliubov transformation](../../../../bogoliubov-transformation.md) gives

$$
\alpha_p=u_pc_p-i v_pc_{-p}^\dagger,\qquad
\alpha_{-p}=u_pc_{-p}+i v_pc_p^\dagger.
$$

Both annihilate the normalized pair state $(u_p+i v_pc_p^\dagger c_{-p}^\dagger)|0\rangle$. For example, applying $\alpha_p$ produces the two cancelling terms $i u_pv_pc_{-p}^\dagger|0\rangle$. Thus

$$
\boxed{|\Omega\rangle=\prod_{p>0}\left(u_p+i v_pc_p^\dagger c_{-p}^\dagger\right)|0\rangle,\qquad c_0|\Omega\rangle=0.}
$$

The factors have even [fermion parity](../../../../fermion-parity.md) and commute for disjoint momentum pairs. Each normalized factor is a [superposition](../../../../superposition-principle.md) of zero and two [fermions](../../../../fermion.md), whose pair-occupation [probability](../../../../probability.md) is $v_p^2$. Therefore

$$
\boxed{\langle\Omega|\widehat N|\Omega\rangle=2\sum_{p>0}v_p^2=\sum_{p>0}\left(1-\frac{\epsilon(p)}{E_p}\right).}
$$

There is no zero-mode contribution. For fixed $L$, the [sum](../../../../sum.md) converges since $v_p^2=O(p^{-4})$.

A normalized simple excited state is $|k\rangle=\alpha_k^\dagger|\Omega\rangle$ for $k>0$. Its [excitation energy](../../../../excitation-energy.md) is $E_k$, and its total [momentum](../../../../momentum-split.md) is $k$: both terms in $\alpha_k^\dagger=u_kc_k^\dagger+i v_kc_{-k}$ add momentum $k$. Acting on the $k,-k$ pair gives

$$
\alpha_k^\dagger\left(u_k+i v_kc_k^\dagger c_{-k}^\dagger\right)|0\rangle
=(u_k^2+v_k^2)c_k^\dagger|0\rangle=c_k^\dagger|0\rangle.
$$

The affected pair now contains exactly one [fermion](../../../../fermion.md) instead of mean number $2v_k^2$; all other pairs are unchanged. Consequently

$$
\boxed{\langle k|\widehat N|k\rangle=\langle\widehat N\rangle_\Omega+1-2v_k^2
=\langle\widehat N\rangle_\Omega+\frac{\epsilon(k)}{E_k}.}
$$

This is the [fermion number of a Bogoliubov excitation](../../../../fermion-number-of-a-bogoliubov-excitation.md). Its change in mean [fermion number](../../../../fermion-number.md) lies between zero and one for $\mu>0$, with the value one at $\Delta=0$. The [Bogoliubov quasiparticle](../../../../bogoliubov-quasiparticle.md) coherently mixes adding a [fermion](../../../../fermion.md) and removing the opposite-momentum [fermion](../../../../fermion.md); it is not an eigen-excitation of the original [fermion number operator](../../../../fermion-number-operator.md). Indeed,

$$
[\widehat N,H]=2i\Delta\sum_{p>0}\left(c_p^\dagger c_{-p}^\dagger+c_{-p}c_p\right),
$$

so [fermion number](../../../../fermion-number.md) is not conserved when $\Delta\ne0$, while [fermion parity](../../../../fermion-parity.md) is conserved. The generally noninteger change is an [expectation value](../../../../expectation-value.md) in a coherent paired background, rather than a fractional eigenvalue of the [fermion number operator](../../../../fermion-number-operator.md). In the weak-pairing limit at fixed $k$, it tends to one, as expected for an ordinary added [fermion](../../../../fermion.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

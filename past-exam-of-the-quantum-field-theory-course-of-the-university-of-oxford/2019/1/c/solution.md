<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define $E_{\mathbf p}=\sqrt{\kappa^2|\mathbf p|^4+m^2}$ and $\int_{\mathbf p}=\int d^3p/(2\pi)^3$. The Hermitian [quantum field](../../../../quantum-field.md) has the [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md)

$$
\boxed{\phi(t,\mathbf x)=\int_{\mathbf p}\frac1{\sqrt{2E_{\mathbf p}}}
\left[a_{\mathbf p}e^{-iE_{\mathbf p}t+i\mathbf p\cdot\mathbf x}
+a_{\mathbf p}^\dagger e^{iE_{\mathbf p}t-i\mathbf p\cdot\mathbf x}\right],}
$$

where the [annihilation operators](../../../../annihilation-operator.md) and [creation operators](../../../../creation-operator.md) obey the bosonic [canonical commutation relations](../../../../canonical-commutation-relation.md)

$$
\boxed{[a_{\mathbf p},a_{\mathbf q}^\dagger]=(2\pi)^3\delta^{(3)}(\mathbf p-\mathbf q),\qquad
[a_{\mathbf p},a_{\mathbf q}]=[a_{\mathbf p}^\dagger,a_{\mathbf q}^\dagger]=0.}
$$

Because $\pi=\dot\phi$, its [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md) is

$$
\pi(t,\mathbf x)=-i\int_{\mathbf p}\sqrt{\frac{E_{\mathbf p}}2}
\left[a_{\mathbf p}e^{-iE_{\mathbf p}t+i\mathbf p\cdot\mathbf x}
-a_{\mathbf p}^\dagger e^{iE_{\mathbf p}t-i\mathbf p\cdot\mathbf x}\right].
$$

The two nonzero cross [commutators](../../../../commutator.md) then give

$$
[\phi(t,\mathbf x),\pi(t,\mathbf y)]
=\frac i2\int_{\mathbf p}\left[e^{i\mathbf p\cdot(\mathbf x-\mathbf y)}+e^{-i\mathbf p\cdot(\mathbf x-\mathbf y)}\right]
=i\delta^{(3)}(\mathbf x-\mathbf y),
$$

and the equal-time field-field and momentum-momentum [commutators](../../../../commutator.md) vanish. This verifies the factor $1/\sqrt{2E_{\mathbf p}}$ without requiring [Lorentz invariance](../../../../lorentz-invariance.md).

Substitution into the [Hamiltonian](../../../../hamiltonian.md), followed by [normal ordering](../../../../normal-ordering.md), yields

$$
\boxed{{:H:}=\int_{\mathbf p}E_{\mathbf p}a_{\mathbf p}^\dagger a_{\mathbf p}.}
$$

Consequently $[{:H:},a_{\mathbf p}^\dagger]=E_{\mathbf p}a_{\mathbf p}^\dagger$: one application of a [creation operator](../../../../creation-operator.md) adds precisely the required [quasiparticle](../../../../quasiparticle.md) [energy](../../../../energy-split.md). Before [normal ordering](../../../../normal-ordering.md) there is the usual constant zero-point [vacuum energy](../../../../vacuum-energy.md). If $m=0$, the exactly zero-[momentum](../../../../momentum-split.md) mode has $E_{\mathbf0}=0$ and is a free canonical coordinate, not an oscillator with a normalizable oscillator [vacuum state](../../../../vacuum-state.md); in a finite box handle that mode separately or introduce a small positive [mass](../../../../mass.md). The formula applies directly to all modes with $E_{\mathbf p}>0$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

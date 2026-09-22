<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\int_{\mathbf p}=\int d^3p/(2\pi)^3$. The [conjugate momentum](../../../../canonical-momentum.md) [fields](../../../../field.md) are $\pi_\phi=\dot\phi^\dagger$ and $\pi_{\phi^\dagger}=\dot\phi$. Inserting the given [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md) into $i\int d^3x(\dot\phi^\dagger\phi-\phi^\dagger\dot\phi)$ produces spatial [Dirac delta](../../../../dirac-delta-function.md) factors. The $b^\dagger c^\dagger$ and $cb$ terms vanish after integration: they contain $\omega_{\mathbf p}-\omega_{\mathbf q}$ on $\delta^3(\mathbf p+\mathbf q)$, and $\omega_{-\mathbf p}=\omega_{\mathbf p}$. The number-conserving terms instead add their two frequency factors, cancelling the mode normalization. The un-subtracted ordered expression is

$$
Q_{\mathrm{raw}}=\int_{\mathbf p}\left(c_{\mathbf p}c_{\mathbf p}^\dagger-b_{\mathbf p}^\dagger b_{\mathbf p}\right)
=\int_{\mathbf p}\left(c_{\mathbf p}^\dagger c_{\mathbf p}-b_{\mathbf p}^\dagger b_{\mathbf p}\right)
+\int_{\mathbf p}(2\pi)^3\delta^3(0).
$$

The last term is an infinite [vacuum](../../../../vacuum.md) constant, not a finite physical [vacuum](../../../../vacuum.md) charge. Choosing the [Fock vacuum](../../../../fock-vacuum.md) to have zero [Noether charge](../../../../noether-charge.md), equivalently using [normal ordering](../../../../normal-ordering.md), gives

$$
\boxed{Q=\int_{\mathbf p}\left(c_{\mathbf p}^\dagger c_{\mathbf p}-b_{\mathbf p}^\dagger b_{\mathbf p}\right)=N_c-N_b.}
$$

A state containing $n_c$ quanta created by $c^\dagger$ and $n_b$ by $b^\dagger$ has [Noether charge](../../../../noether-charge.md) $n_c-n_b$. Thus the two families describe opposite unit [Noether charges](../../../../noether-charge.md); with this source's current the $c^\dagger$ quantum has positive [Noether charge](../../../../noether-charge.md) and the $b^\dagger$ quantum negative [Noether charge](../../../../noether-charge.md). This is an internal [Noether charge](../../../../noether-charge.md); identifying it with [electric charge](../../../../electric-charge-split.md) requires a specified electromagnetic [coupling](../../../../coupling.md). The [vacuum subtraction of a complex scalar charge](../../../../vacuum-subtraction-of-a-complex-scalar-charge.md) leaves all [commutators](../../../../commutator.md) unchanged.[Section 2.5, complex scalar fields and their opposite-charge oscillator families; the phase convention fixes the overall sign](../../../../quantum-field-theory-by-david-tong.md)

**Scope of the expansion:** a fixed-frequency expansion with time-independent oscillator coefficients is the free-field or asymptotic-field form. For arbitrary interacting $f$, it can be used as canonical oscillator coordinates at a chosen time, rather than as the exact interacting time dependence. For example, $f(s)=m^2s+\lambda s^2$ gives $(\Box+m^2)\phi+2\lambda\phi^*\phi\phi=0$, which a generic free plane-wave superposition does not satisfy. The [Noether charge](../../../../noether-charge.md) and its generator [action](../../../../action.md) remain valid in the interacting theory; the [symmetry](../../../../symmetry-physics.md) does not depend on using a free [Hamiltonian](../../../../hamiltonian.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

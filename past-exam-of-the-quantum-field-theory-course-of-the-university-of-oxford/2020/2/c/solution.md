<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the combinations $a_\pm=a\pm b$ at each [momentum](../../../../momentum-split.md). Part [a](../a.md) gives $[Q,a_+]=0$, $[Q,a_-]=-2a_-$, while their [creation operators](../../../../creation-operator.md) obey $[Q,a_+^\dagger]=0$, $[Q,a_-^\dagger]=2a_-^\dagger$. Applying [b](../b.md) gives

$$
\begin{aligned}
C_\lambda a C_\lambda^\dagger
&=\frac{1+e^{-2i\lambda}}2a+\frac{1-e^{-2i\lambda}}2b,\\
C_\lambda b C_\lambda^\dagger
&=\frac{1-e^{-2i\lambda}}2a+\frac{1+e^{-2i\lambda}}2b.
\end{aligned}
$$

The [creation operators](../../../../creation-operator.md) transform by the [Hermitian adjoint](../../../../adjoint-operator.md) formulas with $e^{+2i\lambda}$. At $\lambda=\pi/2$, both exponentials are $-1$, so

$$
\boxed{Ca_{\mathbf p}C^\dagger=b_{\mathbf p},\quad
Cb_{\mathbf p}C^\dagger=a_{\mathbf p},\quad
Ca_{\mathbf p}^\dagger C^\dagger=b_{\mathbf p}^\dagger,\quad
Cb_{\mathbf p}^\dagger C^\dagger=a_{\mathbf p}^\dagger,\qquad C=C_{\pi/2}.}
$$

Substituting into the fixed-time [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md) of the [complex scalar field](../../../../complex-scalar-field.md) gives

$$
C\phi(\mathbf x)C^\dagger
=\int_{\mathbf p}\frac{a_{-\mathbf p}^\dagger+b_{\mathbf p}}{\sqrt{2E_{\mathbf p}}}
 e^{i\mathbf p\cdot\mathbf x}
=\phi^\dagger(\mathbf x).
$$

Thus $C$ exchanges particles and [antiparticles](../../../../antiparticle.md), as required for [charge conjugation](../../../../charge-conjugation.md). To see the charge reversal explicitly, the conserved charge $Q_{\rm em}=\int_{\mathbf p}(a_{\mathbf p}^\dagger a_{\mathbf p}-b_{\mathbf p}^\dagger b_{\mathbf p})$ obeys $CQ_{\rm em}C^\dagger=-Q_{\rm em}$. The generator $Q$ in the question is distinct from this charge.

The two occupation terms in the [Hamiltonian](../../../../hamiltonian.md) are exchanged, with the same [relativistic energy](../../../../relativistic-energy.md) $E_{\mathbf p}$, and therefore

$$
\boxed{CHC^\dagger=H.}
$$

In fact $[Q,H]=0$ because its mixing terms exchange equal-[energy](../../../../energy-split.md) modes. With [normal ordering](../../../../normal-ordering.md), $:Q:=2\int_{\mathbf p}c_{-,\mathbf p}^\dagger c_{-,\mathbf p}$ for $c_-=(a-b)/\sqrt2$. Then $C=e^{i\pi N_-}$ fixes the [vacuum state](../../../../vacuum-state.md) and satisfies $C^2=1$. The construction is a [bosonic species-swap generator](../../../../bosonic-species-swap-generator.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

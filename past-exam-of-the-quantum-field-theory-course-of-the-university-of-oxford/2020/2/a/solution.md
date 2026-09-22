<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\int_{\mathbf p}=\int d^3p/(2\pi)^3$ and $d_{\mathbf p}=a_{\mathbf p}-b_{\mathbf p}$. The nonzero [canonical commutation relations](../../../../canonical-commutation-relation.md) are

$$
[a_{\mathbf p},a_{\mathbf q}^\dagger]
=[b_{\mathbf p},b_{\mathbf q}^\dagger]
=(2\pi)^3\delta^{(3)}(\mathbf p-\mathbf q),
$$

with cross-species brackets zero. The [commutator product rule](../../../../commutator-product-rule.md) gives

$$
\begin{aligned}
[Q,a_{\mathbf q}]&=\int_{\mathbf p}d_{\mathbf p}[d_{\mathbf p}^\dagger,a_{\mathbf q}]=-d_{\mathbf q},\\
[Q,b_{\mathbf q}]&=\int_{\mathbf p}d_{\mathbf p}[d_{\mathbf p}^\dagger,b_{\mathbf q}]=+d_{\mathbf q},\\
[Q,a_{\mathbf q}^\dagger]&=\int_{\mathbf p}[d_{\mathbf p},a_{\mathbf q}^\dagger]d_{\mathbf p}^\dagger=d_{\mathbf q}^\dagger,\\
[Q,b_{\mathbf q}^\dagger]&=\int_{\mathbf p}[d_{\mathbf p},b_{\mathbf q}^\dagger]d_{\mathbf p}^\dagger=-d_{\mathbf q}^\dagger.
\end{aligned}
$$

Linearity of the [commutator](../../../../commutator.md) now yields, for the real coefficient $s$,

$$
\boxed{\begin{aligned}
[Q,a_{\mathbf q}+sb_{\mathbf q}]&=-(1-s)(a_{\mathbf q}-b_{\mathbf q}),\\
[Q,a_{\mathbf q}^\dagger+sb_{\mathbf q}^\dagger]&=(1-s)(a_{\mathbf q}^\dagger-b_{\mathbf q}^\dagger).
\end{aligned}}
$$

Strictly, the printed $Q$ contains an infinite constant in continuum [Fock space](../../../../fock-space.md). Work first with finitely many modes, or replace it by its [normal ordering](../../../../normal-ordering.md) $:Q:=\int_{\mathbf p}d_{\mathbf p}^\dagger d_{\mathbf p}$. Their difference is a constant, so every displayed [commutator](../../../../commutator.md) and every conjugation below is unchanged. The latter convention fixes the [vacuum state](../../../../vacuum-state.md) phase without an infinite phase ambiguity.

## ↑ Ancestors (12)

1. [A](../a.md)
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

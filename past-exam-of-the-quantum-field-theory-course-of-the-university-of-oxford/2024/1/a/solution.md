<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $\int_{\mathbf p}=\int d^3\mathbf p/(2\pi)^3$. The [canonical commutation relations](../../../../canonical-commutation-relation.md) and the product rule for a [commutator](../../../../commutator.md) give

$$
[a_{\mathbf p},a_{\mathbf q}^\dagger a_{\mathbf q}]=(2\pi)^3\delta^3(\mathbf p-\mathbf q)a_{\mathbf q},\qquad
[b_{\mathbf p}^\dagger,b_{\mathbf q}^\dagger b_{\mathbf q}]=-(2\pi)^3\delta^3(\mathbf p-\mathbf q)b_{\mathbf q}^\dagger.
$$

The other-species terms vanish. Integrating the [Dirac delta distributions](../../../../dirac-delta-function.md) in the [Hamiltonian](../../../../hamiltonian.md) therefore gives

$$
[a_{\mathbf p},H]=E_p a_{\mathbf p},\qquad [b_{-\mathbf p}^\dagger,H]=-E_p b_{-\mathbf p}^\dagger,
$$

where $E_{-p}=E_p$. Consequently the [complex scalar field](../../../../complex-scalar-field.md) satisfies

$$
[\phi(t,\mathbf x),H]=\int_{\mathbf p}\frac{E_p}{\sqrt{2E_p}}\left(-b_{-\mathbf p}^\dagger e^{iE_pt}+a_{\mathbf p}e^{-iE_pt}\right)e^{i\mathbf p\cdot\mathbf x}.
$$

Direct [differentiation](../../../../differentiation.md) of the time factors gives the same expression, proving the [Heisenberg equation of motion](../../../../heisenberg-equation-of-motion.md)

$$
\boxed{i\partial_t\phi(t,\mathbf x)=[\phi(t,\mathbf x),H].}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

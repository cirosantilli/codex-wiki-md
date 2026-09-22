<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Read the unsuperscripted $a_{\mathbf p}$ in the printed [Hamiltonian](../../../../hamiltonian.md) as $a_{\mathbf p}^s$: the repeated [spin](../../../../spin.md) label is otherwise missing. Relabel $\mathbf p\mapsto-\mathbf p$ in its antiparticle term, and insert both projections from [c](../c.md). Keeping the original operator ordering gives

$$
\begin{aligned}
H&=\int\frac{d^3p}{(2\pi)^3}\,
\widetilde\psi^\dagger(t,\mathbf p)
\left[\frac12\sum_s\left(u^s(\mathbf p)u^{s\dagger}(\mathbf p)
-v^s(-\mathbf p)v^{s\dagger}(-\mathbf p)\right)\right]
\widetilde\psi(t,\mathbf p)\\
&=\int\frac{d^3p}{(2\pi)^3}\,
\widetilde\psi^\dagger(t,\mathbf p)
(\boldsymbol\alpha\cdot\mathbf p+\beta m)
\widetilde\psi(t,\mathbf p).
\end{aligned}
$$

The difference of the two [orthogonal projectors](../../../../orthogonal-projection.md) in [a](../a.md) is $h(\mathbf p)/E$, explaining the cancellation of the factors $E$. Under inverse [Fourier transformation](../../../../fourier-transform-split.md), $\mathbf p$ becomes $-i\boldsymbol\nabla$ acting on $\psi$. Hence

$$
\boxed{H=\int d^3x\,\mathcal H,\qquad
\mathcal H=\psi^\dagger(-i\boldsymbol\alpha\cdot\boldsymbol\nabla+\beta m)\psi
=\bar\psi(-i\gamma^i\partial_i+m)\psi.}
$$

Spatial indices run from $1$ to $3$. This is the local [Hamiltonian density](../../../../hamiltonian-density.md) of the free [Dirac field](../../../../dirac-field.md). It also follows from $\mathcal H=\pi\dot\psi-\mathcal L$ with $\pi=i\psi^\dagger$.

The original antiparticle term is $-bb^\dagger$, so the result retains its infinite additive [vacuum energy](../../../../vacuum-energy.md). If the [Hamiltonian](../../../../hamiltonian.md) is [normal-ordered](../../../../normal-ordering.md), its occupation-number expression becomes $\int d^3p/(2\pi)^3\,E\sum_s(a^{s\dagger}a^s+b^{s\dagger}b^s)$ and its local expression is $:\!\mathcal H\!:$, with the same subtraction. The displayed unsymmetrized [Hamiltonian density](../../../../hamiltonian-density.md) is [Hermitian](../../../../hermitian-operator.md) after spatial integration under vanishing boundary terms; a manifestly [Hermitian](../../../../hermitian-operator.md) local form replaces the derivative term by $-\tfrac i2\psi^\dagger\boldsymbol\alpha\cdot\overleftrightarrow{\boldsymbol\nabla}\psi$ and differs by a spatial [divergence](../../../../divergence.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

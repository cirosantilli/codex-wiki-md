<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the constant [Dirac gamma matrix](../../../../gamma-matrices.md) combinations $\alpha^k=\gamma^0\gamma^k$ and $\beta=\gamma^0$. The [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) is

$$
H=\int d^3y\,\psi_b^\dagger(\mathbf y)
(-i\alpha^k_{bc}\partial_{y^k}+m\beta_{bc})\psi_c(\mathbf y).
$$

Evaluate its [commutator](../../../../commutator.md) with $n(\mathbf x)$ using the bilocal result in [a](../a.md). The [mass term](../../../../mass-term.md) cancels immediately when $\mathbf z=\mathbf y$, because its two [Dirac delta distributions](../../../../dirac-delta-function.md) coincide. For the derivative term first keep the two points distinct:

$$
C(\mathbf x)=-i\int d^3y\,\alpha^k_{bc}\left.
\partial_{z^k}\left\{[\delta^{(3)}(\mathbf x-\mathbf y)-\delta^{(3)}(\mathbf x-\mathbf z)]
\psi_b^\dagger(\mathbf y)\psi_c(\mathbf z)\right\}\right|_{\mathbf z=\mathbf y}.
$$

The terms in which the derivative acts on $\psi_c$ cancel against each other; the derivative of the second [Dirac delta distribution](../../../../dirac-delta-function.md) remains. Thus

$$
C(\mathbf x)=i\int d^3y\,\psi^\dagger(\mathbf y)\alpha^k\psi(\mathbf y)
\partial_{y^k}\delta^{(3)}(\mathbf x-\mathbf y)
=-i\partial_{x^k}[\psi^\dagger(\mathbf x)\alpha^k\psi(\mathbf x)].
$$

The last equality is [integration by parts](../../../../integration-by-parts.md), or the defining derivative rule for a [distribution](../../../../distribution-mathematical-analysis.md). Consequently the literal [conserved current](../../../../conserved-current.md) whose [divergence](../../../../divergence.md) equals $C$ is

$$
\boxed{C=\boldsymbol\nabla\cdot\mathbf J,\qquad
J^k=-i\psi^\dagger\alpha^k\psi=-i\bar\psi\gamma^k\psi.}
$$

Because a [commutator](../../../../commutator.md) of two [Hermitian operators](../../../../hermitian-operator.md) is anti-Hermitian, this $\mathbf J$ includes $-i$. The physical Hermitian [Dirac current](../../../../dirac-current.md) is instead $j^k=\bar\psi\gamma^k\psi$, so $C=-i\boldsymbol\nabla\cdot\mathbf j$. The [Heisenberg equation of motion](../../../../heisenberg-equation-of-motion.md) now gives

$$
\boxed{\partial_t n=i[H,n]=-iC=-\boldsymbol\nabla\cdot\mathbf j,\qquad
j^\mu=\bar\psi\gamma^\mu\psi.}
$$

This establishes the [continuity equation](../../../../continuity-equation.md) directly from the required [commutator](../../../../commutator.md), without assuming the [Dirac equation](../../../../dirac-equation.md) or invoking the [Noether theorem](../../../../noether-theorem.md) as a substitute for the computation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For arbitrary [linear operators](../../../../linear-operator.md), expansion of the [anticommutators](../../../../anticommutator.md) gives

$$
\{X,Y\}Z-Y\{X,Z\}=(XY+YX)Z-Y(XZ+ZX)=XYZ-YZX=[X,YZ].
$$

Now use the [commutator product rule](../../../../commutator-product-rule.md) $[VX,W]=V[X,W]+[V,W]X$, with $W=YZ$, twice. The result is

$$
\boxed{[VX,YZ]=V\{X,Y\}Z-VY\{X,Z\}+\{V,Y\}ZX-Y\{V,Z\}X.}
$$

No grading assumption is needed for these algebraic identities.

For the [Dirac field](../../../../dirac-field.md), supplement the supplied equal-time [canonical anticommutation relations](../../../../canonical-anticommutation-relations.md) with $\{\psi_a(x),\psi_b(y)\}=\{\psi_a^\dagger(x),\psi_b^\dagger(y)\}=0$. Define the [fermion number](../../../../fermion-number.md) density $n(\mathbf x)=\sum_a\psi_a^\dagger(\mathbf x)\psi_a(\mathbf x)$. In the preceding identity take $V=\psi_a^\dagger(\mathbf x)$, $X=\psi_a(\mathbf x)$, $Y=\psi_b^\dagger(\mathbf y)$, $Z=\psi_c(\mathbf z)$ and sum over $a$. Only its first and last [anticommutators](../../../../anticommutator.md) survive, giving

$$
\boxed{[n(\mathbf x),\psi_b^\dagger(\mathbf y)\psi_c(\mathbf z)]
=\left[\delta^{(3)}(\mathbf x-\mathbf y)-\delta^{(3)}(\mathbf x-\mathbf z)\right]
\psi_b^\dagger(\mathbf y)\psi_c(\mathbf z).}
$$

This is an identity of operator-valued [distributions](../../../../distribution-mathematical-analysis.md). Point splitting, or smearing with test functions, gives a precise meaning to coincident bilinears. [Normal ordering](../../../../normal-ordering.md) only subtracts a constant from the density and does not alter this [commutator](../../../../commutator.md).

## ↑ Ancestors (12)

1. [A](../a.md)
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

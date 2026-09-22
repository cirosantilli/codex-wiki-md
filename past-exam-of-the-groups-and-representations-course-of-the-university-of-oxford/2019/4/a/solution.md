<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a differentiable curve $Q(t)\in SO(5)$ with $Q(0)=I_5$, differentiate $Q(t)^TQ(t)=I_5$. Its tangent [matrix](../../../../matrix.md) $X=Q'(0)$ is real and satisfies $X^T+X=0$. Conversely the [matrix exponential](../../../../matrix-exponential.md) of any real [antisymmetric matrix](../../../../skew-symmetric-matrix.md) is orthogonal, and $\det e^{tX}=e^{t\operatorname{tr}X}=1$ because $\operatorname{tr}X=0$. Hence the real [Special orthogonal Lie algebra](../../../../special-orthogonal-lie-algebra.md) is

$$
\boxed{\mathfrak{so}(5)=\{X\in M_5(\mathbb R):X^T=-X\},\qquad [X,Y]=XY-YX.}
$$

Let $E_{ab}$ denote a [matrix unit](../../../../matrix-unit.md). A simple real [basis](../../../../basis.md) is

$$
\boxed{M_{ab}=E_{ab}-E_{ba},\qquad 1\leq a<b\leq5.}
$$

Each independent entry above the diagonal supplies one real parameter, giving $\binom52=10$ parameters. The [commutator](../../../../commutator.md) of two [basis](../../../../basis.md) [matrices](../../../../matrix.md) is

$$
[M_{ab},M_{cd}]=\delta_{bc}M_{ad}-\delta_{ac}M_{bd}-\delta_{bd}M_{ac}+\delta_{ad}M_{bc},
$$

where $M_{ba}=-M_{ab}$ and $M_{aa}=0$.

A [Cartan subalgebra](../../../../cartan-subalgebra.md) is spanned by the commuting [matrices](../../../../matrix.md) $M_{12},M_{34}$, which generate independent rotations in two orthogonal planes. A generic $h=aM_{12}+bM_{34}$, with $ab(a^2-b^2)\ne0$, has distinct complex [eigenvalues](../../../../eigenvalue.md) $ia,-ia,ib,-ib,0$. A real [antisymmetric matrix](../../../../skew-symmetric-matrix.md) commuting with it preserves those two planes and the remaining line; it is a multiple of the rotation in each plane and is zero on the line. Thus the commuting [Lie subalgebra](../../../../lie-subalgebra.md) has [dimension](../../../../dimension-vector-space.md) two and is maximal toral. Therefore

$$
\boxed{\dim_{\mathbb R}\mathfrak{so}(5)=10,\qquad\operatorname{rank}\mathfrak{so}(5)=2.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)

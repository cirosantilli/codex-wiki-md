<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Differentiate a curve $U(t)\in SU(4)$ through $U(0)=I$, writing $X=U'(0)$. Differentiating $U(t)^\dagger U(t)=I$ gives $X^\dagger+X=0$; differentiating $\det U(t)=1$ gives $\operatorname{tr}X=0$. Conversely, for every [anti-Hermitian matrix](../../../../skew-hermitian-matrix.md) $X$ with zero [trace](../../../../matrix-trace.md), the [matrix exponential](../../../../matrix-exponential.md) $e^{tX}$ is unitary and has [determinant](../../../../determinant.md) $e^{t\operatorname{tr}X}=1$. Thus the real [Lie algebra](../../../../lie-algebra-split.md) is

$$
\boxed{\mathfrak{su}(4)=\{X\in M_4(\mathbb C):X^\dagger=-X,\ \operatorname{tr}X=0\},\qquad [X,Y]=XY-YX.}
$$

The [commutator](../../../../commutator.md) again has zero [trace](../../../../matrix-trace.md) and is [anti-Hermitian](../../../../skew-hermitian-matrix.md), so this set is closed under the [Lie bracket](../../../../lie-bracket.md). Let $E_{jk}$ be the [matrix units](../../../../matrix-unit.md). A convenient real [basis](../../../../basis.md) is

$$
\boxed{A_{jk}=E_{jk}-E_{kj},\quad B_{jk}=i(E_{jk}+E_{kj})\quad(1\leq j<k\leq4),\qquad H_a=i(E_{aa}-E_{a+1,a+1})\quad(a=1,2,3).}
$$

There are six independent $A_{jk}$, six independent $B_{jk}$, and three independent $H_a$. Every permitted off-diagonal complex entry is supplied by one real combination of $A_{jk},B_{jk}$; the imaginary diagonal entries have one [trace](../../../../matrix-trace.md) constraint and are spanned by the $H_a$. Consequently

$$
\boxed{\dim_{\mathbb R}\mathfrak{su}(4)=15,\qquad\operatorname{rank}\mathfrak{su}(4)=3.}
$$

For the [rank of a semisimple Lie algebra](../../../../rank-of-a-semisimple-lie-algebra.md), the diagonal [Cartan subalgebra](../../../../cartan-subalgebra.md) consists of $i\operatorname{diag}(t_1,t_2,t_3,t_4)$ with real $t_i$ and $\sum_i t_i=0$, of [dimension](../../../../dimension-vector-space.md) three. Commuting [anti-Hermitian matrices](../../../../skew-hermitian-matrix.md) are simultaneously unitarily diagonalizable, so no larger commuting toral [Lie subalgebra](../../../../lie-subalgebra.md) exists. In the common physics convention one uses the [Hermitian](../../../../hermitian-operator.md) generators $-iA_{jk},-iB_{jk},-iH_a$ and writes [group](../../../../group-split.md) elements as $e^{itT}$; these are the same generators with the factor of $i$ moved into the exponential.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [4](../../4.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

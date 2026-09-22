<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the [monomial basis](../../../monomial-basis.md) $e_k=x^{n-k}y^k$, $0\leq k\leq n$. Direct differentiation gives

$$
Pe_k=k e_{k-1},\qquad Qe_k=(n-k)e_{k+1},
$$

with the endpoint terms zero. Repeated application therefore gives $P^{n+1}=Q^{n+1}=0$, while $P^ne_n=n!e_0\neq0$ and $Q^ne_0=n!e_n\neq0$. Each [nilpotency index](../../../nilpotency-index.md) is exactly $n+1$, so

$$
\boxed{m_P(t)=m_Q(t)=t^{n+1}.}
$$

Next

$$
PQe_k=(n-k)(k+1)e_k,\qquad
QPe_k=k(n-k+1)e_k,
$$

and hence $(PQ-QP)e_k=(n-2k)e_k$. These $n+1$ real [eigenvalues](../../../eigenvalue.md) are distinct. A [polynomial](../../../polynomial-split.md) annihilates this operator exactly when it vanishes at all of them, giving

$$
\boxed{m_{PQ-QP}(t)=\prod_{k=0}^n(t-(n-2k)).}
$$

The [commutator](../../../commutator.md) is diagonal in the displayed [monomial basis](../../../monomial-basis.md). Since $n\geq1$, $P,Q$ are nonzero [nilpotent linear map](../../../nilpotent-linear-map.md); a [diagonalizable](../../../diagonalizable-matrix.md) nilpotent map would have a [diagonal matrix](../../../diagonal-matrix.md) with all [eigenvalues](../../../eigenvalue.md) zero and thus be the zero map. Therefore **only $PQ-QP$ is [diagonalizable](../../../diagonalizable-matrix.md)**. The calculation realizes [raising and lowering on binary homogeneous polynomials](../../../raising-and-lowering-on-binary-homogeneous-polynomials.md).

## ↑ Ancestors (11)

1. [2](../2.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

<h1 id="algebra/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Expanding the [determinant](../../../../../determinant.md) along the second column gives

$$
\chi_X(t)=(t+3)(t-b)(t-2).
$$

If $b\notin\{-3,2\}$, there are three distinct real [eigenvalues](../../../../../eigenvalue.md). Part (b)(ii) gives a nonzero [eigenvector](../../../../../eigenvector.md) for each, and part (b)(i) makes them independent. They form a basis, so the matrix is diagonalisable.

When $b=-3$,

$$
X+3I=\begin{pmatrix}0&0&0\\2a&0&a\\10&0&5\end{pmatrix}
$$

has rank one for every $a$: the third row is nonzero, and the second row is $a/5$ times the third. Therefore the [eigenspace](../../../../../eigenspace.md) for $-3$ has dimension two. The [eigenvalue](../../../../../eigenvalue.md) $2$ provides at least one further independent [eigenvector](../../../../../eigenvector.md) by part (b), so again there is an [eigenbasis](../../../../../eigenbasis.md).

When $b=2$,

$$
X-2I=\begin{pmatrix}-5&0&0\\2a&0&a\\10&0&0\end{pmatrix}.
$$

Its rank is one if $a=0$ and two otherwise. Thus the [eigenspace](../../../../../eigenspace.md) for $2$ has dimension two exactly when $a=0$. For $a\neq0$ it has dimension one, while the [eigenspace](../../../../../eigenspace.md) for $-3$ also has dimension one, since $X+3I$ then has rank two. There are no other [eigenvalues](../../../../../eigenvalue.md) by the [characteristic polynomial](../../../../../characteristic-polynomial.md). A diagonal matrix in an [eigenbasis](../../../../../eigenbasis.md) would need three independent [eigenvectors](../../../../../eigenvector.md), whereas these two [eigenspaces](../../../../../eigenspace.md) supply only two; diagonalisation is impossible. Conversely, at $a=0$ their dimensions add to three and part (b) makes their sum direct. Therefore

$$
\boxed{X_{a,b}\text{ is diagonalisable}\quad\Longleftrightarrow\quad b\neq2\text{ or }a=0.}
$$

The argument uses only the [determinant](../../../../../determinant.md), rank-nullity, the established direct-sum result, and the definition of diagonalisation.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [1](../../1.md)
3. [Algebra](../../../algebra.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

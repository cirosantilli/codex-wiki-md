<h1 id="9g/solution">Solution</h1>

↑ **Parent:** [9G](../9g.md)

The [structure theorem for finitely generated modules over a principal ideal domain](../../../../../structure-theorem-for-finitely-generated-modules-over-a-principal-ideal-domain.md) applies because every [Euclidean domain](../../../../../euclidean-domain.md) is a [principal ideal domain](../../../../../principal-ideal-domain.md). It says that a finitely generated $R$-module is isomorphic to

$$
R^s\oplus R/(d_1)\oplus\cdots\oplus R/(d_k),
\qquad d_1\mid d_2\mid\cdots\mid d_k,
$$

where the nonzero nonunits $d_i$ are unique up to multiplication by units. They are the [invariant factors](../../../../../invariant-factors-of-a-linear-operator.md).

For $V_\alpha$, multiplication by $X$ is the [linear map](../../../../../linear-map.md) $\alpha$. Since $V$ is finite-dimensional over $F$, $V_\alpha$ is a finitely generated [torsion module](../../../../../torsion-module.md) over the [polynomial ring](../../../../../polynomial-ring.md) $F[X]$, so it has no free summand. Choosing each invariant factor $a_i$ to be monic gives

$$
V_\alpha\cong\bigoplus_{i=1}^k F[X]/(a_i),
\qquad a_1\mid\cdots\mid a_k.
$$

The basis $1,X,\ldots,X^{\deg a_i-1}$ of each cyclic summand makes multiplication by $X$ a [companion matrix](../../../../../companion-matrix.md). Concatenating these bases therefore puts $\alpha$ in [rational canonical form](../../../../../rational-canonical-form.md).

On $F[X]/(a_i)$, a polynomial annihilates multiplication by $X$ exactly when it is divisible by $a_i$. It follows that the [minimal polynomial](../../../../../minimal-polynomial.md) and [characteristic polynomial](../../../../../characteristic-polynomial.md) are

$$
\boxed{m_\alpha(X)=a_k(X)},
\qquad
\boxed{\chi_\alpha(X)=\prod_{i=1}^k a_i(X)}.
$$

The second identity follows blockwise from the characteristic polynomial of a companion matrix. Since every $a_i$ divides $a_k$, the product $\chi_\alpha$ annihilates every cyclic summand. Thus $\chi_\alpha(\alpha)=0$, which is the [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem.md).

For the displayed matrix, the given generators of $\ker\theta$ are the columns of

$$
XI-A=
\begin{pmatrix}
X&-1&0\\
4&X-4&0\\
2&-1&X-2
\end{pmatrix}.
$$

Elementary row and column operations over $\mathbb R[X]$ give the [Smith normal form](../../../../../smith-normal-form.md)

$$
\operatorname{diag}\bigl(1,X-2,(X-2)^2\bigr).
$$

Consequently the nonunit invariant factors are

$$
\boxed{X-2\quad\text{and}\quad(X-2)^2},
$$

and, as a check,

$$
m_\alpha(X)=(X-2)^2,
\qquad
\chi_\alpha(X)=(X-2)^3.
$$

## ↑ Ancestors (10)

1. [9G](../9g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

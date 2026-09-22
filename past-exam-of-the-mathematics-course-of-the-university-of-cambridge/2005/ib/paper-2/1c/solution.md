<h1 id="1c/solution">Solution</h1>

↑ **Parent:** [1C](../1c.md)

Direct [matrix](../../../../../matrix.md) multiplication gives the multiplication table

$$
J^2=K^2=L^2=-I,\qquad JK=L,\quad KL=J,\quad LJ=K,\qquad KJ=-L,\quad LK=-J,\quad JL=-K.
$$

Together with $I$ acting as the identity, this shows that the product of any two real [linear combinations](../../../../../linear-combination.md) is again a real [linear combination](../../../../../linear-combination.md). Thus $\Omega$ is closed under multiplication. It is the [complex matrix representation of quaternions](../../../../../complex-matrix-representation-of-quaternions.md).

Its general element has the form

$$
\alpha=\begin{pmatrix}a+ib&c+id\\-c+id&a-ib\end{pmatrix}.
$$

If this [matrix](../../../../../matrix.md) is zero, real and imaginary parts of its first row give $a=b=c=d=0$. Hence $I,J,K,L$ are linearly independent over $\mathbb R$ and form a [basis](../../../../../basis.md):

$$
\boxed{\dim_{\mathbb R}\Omega=4.}
$$

Put $v=bJ+cK+dL$. Since distinct [imaginary units](../../../../../imaginary-unit.md) anticommute, the mixed terms in $v^2$ cancel, leaving $v^2=-(b^2+c^2+d^2)I$. Scalars commute with $v$, so

$$
(aI+v)(aI-v)=a^2I-v^2=(a^2+b^2+c^2+d^2)I.
$$

The reversed product is the same. The coefficient is strictly positive for every nonzero element. Consequently

$$
\boxed{\alpha^{-1}=\frac{aI-bJ-cK-dL}{a^2+b^2+c^2+d^2}\in\Omega\qquad(\alpha\ne0).}
$$

This also identifies $\Omega$ as a real noncommutative [division algebra](../../../../../division-algebra.md), not as the full algebra of complex two-by-two [matrices](../../../../../matrix.md).

## ↑ Ancestors (10)

1. [1C](../1c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

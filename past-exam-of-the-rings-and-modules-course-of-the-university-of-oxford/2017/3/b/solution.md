<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [rational canonical form](../../../../rational-canonical-form.md) of $T$ is a block diagonal matrix

$$
C(f_1)\oplus\cdots\oplus C(f_r),\qquad
f_1\mid f_2\mid\cdots\mid f_r,
$$

similar to a matrix of $T$, where the $f_j\in F[t]$ are monic nonconstant polynomials and the sum of their degrees is $\dim V$. They are the [invariant factors of a linear operator](../../../../invariant-factors-of-a-linear-operator.md). The block $C(f_j)$ is the [companion matrix](../../../../companion-matrix.md) for $f_j$, representing multiplication by $t$ on $F[t]/(f_j)$. The invariant factors are uniquely determined by $T$.

Every companion block has a [cyclic vector](../../../../cyclic-vector.md) and therefore has both [minimal polynomial](../../../../minimal-polynomial.md) and [characteristic polynomial](../../../../characteristic-polynomial.md) equal to $f_j$, by part (a). The [determinant of a block diagonal matrix](../../../../determinant-of-a-block-diagonal-matrix.md) is the product of its block determinants, giving

$$
\boxed{c_T(t)=\prod_{j=1}^r f_j(t).}
$$

A polynomial $h$ annihilates the whole matrix exactly when it annihilates every block. On block $j$, dividing $h$ by $f_j$ leaves a remainder of smaller degree; if that remainder annihilated the block without being zero, it would contradict minimality of $f_j$. Thus the annihilation condition is exactly $f_j\mid h$ for every $j$. The monic polynomial of least degree with this property is their [least common multiple](../../../../least-common-multiple.md). The divisibility chain makes this $f_r$, so

$$
\boxed{m_T(t)=f_r(t).}
$$

These are the [minimal and characteristic polynomials from invariant factors](../../../../minimal-and-characteristic-polynomials-from-invariant-factors.md) formulae. On the zero vector space the product is empty and both polynomials are defined to be one.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the rings and modules course of the University of Oxford](../../../split.md)
5. [Rings and modules course of the University of Oxford](../../../../rings-and-modules-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

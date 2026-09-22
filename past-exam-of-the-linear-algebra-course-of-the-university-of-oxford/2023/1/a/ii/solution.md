<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [ii](../ii.md)

All calculations here take place in the [finite field](../../../../../finite-field.md) $F=\mathbb F_3$. For the given [matrix](../../../../../matrix.md) $S$, its [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
\chi_S(x)=\det(xI-S)=x^3+2x^2+2x=xq(x),\qquad q(x)=x^2+2x+2.
$$

The values $q(0),q(1),q(2)$ are $2,2,1$, so this [quadratic polynomial](../../../../../quadratic-polynomial.md) has no [polynomial root](../../../../../root-of-a-polynomial.md) in $F$ and is an [irreducible polynomial](../../../../../irreducible-polynomial.md). Direct calculation gives

$$
q(S)=S^2+2S+2I=
\begin{pmatrix}1&1&0\\1&1&0\\1&1&0\end{pmatrix},
\qquad S q(S)=0.
$$

Neither $S$ nor $q(S)$ is zero. The [Cayley-Hamilton theorem](../../../../../cayley-hamilton-theorem-split.md) says that the [minimal polynomial](../../../../../minimal-polynomial.md) divides $xq(x)$; its proper [monic polynomial](../../../../../monic-polynomial.md) divisors cannot annihilate $S$, so $m_S=xq$.

The two [kernels](../../../../../kernel-of-a-linear-map-split.md) give the required [primary decomposition theorem for linear maps](../../../../../primary-decomposition-theorem-for-linear-maps.md) explicitly:

$$
\boxed{\begin{aligned}
W_1&=\ker S=\operatorname{span}_F\{(1,1,1)^T\},\\
W_2&=\ker q(S)=\{(a,-a,b)^T:a,b\in F\}
=\operatorname{span}_F\{(1,2,0)^T,(0,0,1)^T\}.
\end{aligned}}
$$

The determinant of the [matrix](../../../../../matrix.md) with these three [basis vectors](../../../../../basis-vector.md) as columns is $1$ in $F$, proving $W=W_1\oplus W_2$. To check these are [invariant subspaces](../../../../../invariant-subspace.md), writing $u=(1,2,0)^T$ and $z=(0,0,1)^T$ gives $Su=u+2z$ and $Sz=2u$. Hence the [matrix](../../../../../matrix.md) of the [restriction](../../../../../restriction-mathematics.md) to $W_2$ in the [basis](../../../../../basis.md) $(u,z)$ is

$$
\begin{pmatrix}1&2\\2&0\end{pmatrix},
$$

with [minimal polynomial](../../../../../minimal-polynomial.md) $q$; the nonzero [vector space](../../../../../vector-space-split.md) $W_1$ has zero [restriction](../../../../../restriction-mathematics.md) and [minimal polynomial](../../../../../minimal-polynomial.md) $x$.

## ↑ Ancestors (13)

1. [ii](../ii.md)
2. [a](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the linear algebra course of the University of Oxford](../../../../split.md)
6. [Linear algebra course of the University of Oxford](../../../../../linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

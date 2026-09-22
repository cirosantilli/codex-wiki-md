<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [a](../a.md)

In the [monomial basis](../../../../monomial-basis.md) $\mathcal B=(1,x,x^2,x^3)$ of the [complex vector space](../../../../complex-vector-space.md) $V=\mathbb C[x]_{\leq3}$, the [binomial theorem](../../../../binomial-theorem.md) gives

$$
[T]_{\mathcal B}=
\begin{pmatrix}
1&1&1&1\\
0&1&2&3\\
0&0&1&3\\
0&0&0&1
\end{pmatrix}.
$$

The [characteristic polynomial](../../../../characteristic-polynomial.md) of this [upper triangular matrix](../../../../upper-triangular-matrix.md) is the product of $t$ minus its [diagonal entries](../../../../diagonal-matrix-entry.md), so $\chi_T(t)=(t-1)^4$.

For the [minimal polynomial](../../../../minimal-polynomial.md), set $\Delta=T-I$, the [forward difference](../../../../forward-difference.md) with step one. For a nonconstant [polynomial](../../../../polynomial-split.md) of [polynomial degree](../../../../degree-of-a-polynomial.md) $d$, the [binomial theorem](../../../../binomial-theorem.md) shows that $f(x+1)-f(x)$ has [polynomial degree](../../../../degree-of-a-polynomial.md) $d-1$. Constant [polynomials](../../../../polynomial-split.md) have zero [forward difference](../../../../forward-difference.md). Consequently $\Delta^4=0$ on $V$. To prove that the [nilpotency index](../../../../nilpotency-index.md) is exactly four, compute

$$
\Delta x^3=3x^2+3x+1,\qquad
\Delta^2x^3=6x+6,\qquad
\Delta^3x^3=6\ne0.
$$

It follows that

$$
\boxed{\chi_T(t)=(t-1)^4,\qquad m_T(t)=(t-1)^4.}
$$

If $T$ were [diagonalizable](../../../../diagonalizable-matrix.md), its only [eigenvalue](../../../../eigenvalue.md) would be $1$, and its [diagonal matrix](../../../../diagonal-matrix.md) in an [eigenbasis](../../../../eigenbasis.md) would be $I$. This would make $T=I$, whereas $T(x)=x+1\ne x$. Thus **$T$ is not [diagonalizable](../../../../diagonalizable-matrix.md)**. Equivalently, its [minimal polynomial](../../../../minimal-polynomial.md) has a [repeated root](../../../../multiple-root.md).

## ↑ Ancestors (12)

1. [a](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the linear algebra course of the University of Oxford](../../../split.md)
5. [Linear algebra course of the University of Oxford](../../../../linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

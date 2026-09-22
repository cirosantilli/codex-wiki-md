<h1 id="9c/solution">Solution</h1>

↑ **Parent:** [9C](../9c.md)

Order the states as sandwich $N$, Hall $H$, and own cooking $C$. The [transition matrix](../../../../../stochastic-matrix.md), with current state indexing the row, is

$$
P=\begin{pmatrix}1/2&1/4&1/4\\1/3&1/3&1/3\\1&0&0\end{pmatrix}.
$$

The two probabilities $1/4$ in the first row are unconditional alternatives to the probability $1/2$ of returning. Let $a_n=(P^n)_{HH}$, so $n$ counts days after the initial Hall lunch. Expanding the determinant gives the [characteristic polynomial](../../../../../characteristic-polynomial.md)

$$
\det(\lambda I-P)=\lambda(\lambda-1)(\lambda+1/6).
$$

The three distinct [eigenvalues](../../../../../eigenvalue.md) imply that the sequence has the form

$$
a_n=A+B(-1/6)^n+C0^n,
$$

using the specified $0^0=1$. Directly, $a_0=1$, $a_1=1/3$ and $a_2=7/36$. The last two equations give $A=3/14$ and $B=-5/7$; then $C=3/2$. Consequently

$$
\boxed{a_{60}=\frac3{14}-\frac5{7\,6^{60}}.}
$$

The limiting value is also the Hall entry of the [stationary distribution](../../../../../stationary-distribution.md) $(4/7,3/14,3/14)$. The tiny finite-time correction is retained in the boxed exact probability. Sixty days later means sixty transitions, rather than the sixtieth day including the initial day.

## ↑ Ancestors (10)

1. [9C](../9c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

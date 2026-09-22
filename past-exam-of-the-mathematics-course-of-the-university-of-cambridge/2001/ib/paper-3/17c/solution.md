<h1 id="17c/solution">Solution</h1>

↑ **Parent:** [17C](../17c.md)

Work in the finite-dimensional [vector space](../../../../../vector-space-split.md) $V$ implicit in the requested matrix representation and $n=\dim V$. Put $K_j=\ker\alpha^j$, with $K_0=0$. These form an increasing sequence ending in $K_m=V$, and $\alpha(K_j)\subseteq K_{j-1}$. Choose a [basis](../../../../../basis.md) of $K_1$, extend it to a basis of $K_2$, and continue until a basis of $V$ is obtained. Each basis vector introduced at stage $j$ maps into the span of vectors chosen at earlier stages. Its matrix column can therefore have nonzero entries only in earlier rows. This proves that the matrix is **strictly upper triangular**.

For a strictly upper-triangular $n\times n$ [matrix](../../../../../matrix.md) $N$, a nonzero contribution to $(N^r)_{ij}$ requires an index chain $i<i_1<\cdots<i_{r-1}<j$. No such chain has $n$ links among $n$ indices. Consequently $\boxed{\alpha^n=0}$. An example with exact index four is the [Nilpotent Jordan block](../../../../../nilpotent-jordan-block.md)

$$
\boxed{M=\begin{pmatrix}0&1&0&0\\0&0&1&0\\0&0&0&1\\0&0&0&0\end{pmatrix}.}
$$

Here $M^3$ has entry one in position $(1,4)$ and all others zero, while $M^4=0$.

In the adapted basis, $I+A$ is upper triangular with diagonal entries one, so all its [eigenvalues](../../../../../eigenvalue.md) are one. This does not persist for the product of two such matrices with unrelated adapted bases. Take

$$
A=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad B=\begin{pmatrix}0&0\\1&0\end{pmatrix}.
$$

Both square to zero, but

$$
(I+A)(I+B)=\begin{pmatrix}2&1\\1&1\end{pmatrix}
$$

has [characteristic polynomial](../../../../../characteristic-polynomial.md) $t^2-3t+1$ and [eigenvalues](../../../../../eigenvalue.md) $(3\pm\sqrt5)/2$, neither equal to one. The obstruction is that the two nilpotent matrices need not admit a common triangularizing basis.

## ↑ Ancestors (10)

1. [17C](../17c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

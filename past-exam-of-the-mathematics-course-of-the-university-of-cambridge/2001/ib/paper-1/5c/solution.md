<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

Expansion of the [determinant](../../../../../determinant.md) along the first row gives

$$
\det M=2x^2-(3-x)+2x(1-x)=3(x-1).
$$

Thus **the [matrix](../../../../../matrix.md) is invertible exactly when $x\ne1$**. The minor formed from the first two rows and the last two columns is $-1$, independently of $x$, so the [matrix rank](../../../../../matrix-rank.md) is always at least two. Therefore

$$
\boxed{\operatorname{rank}M=\begin{cases}3,&x\ne1,\\2,&x=1.\end{cases}}
$$

Taking cofactors and transposing them gives the [adjugate matrix](../../../../../adjugate-matrix.md)

$$
\boxed{\operatorname{adj}M=
\begin{pmatrix}
2x&2x-1&-1\\
x-3&x-2&1\\
2x(1-x)&2(1-x^2)&x-1
\end{pmatrix}}.
$$

The [adjugate identity](../../../../../adjugate-identity.md) $M\operatorname{adj}M=(\det M)I$ then gives

$$
\boxed{M^{-1}=\frac1{3(x-1)}\operatorname{adj}M\quad(x\ne1)}.
$$

In particular, the singular case has rank two, rather than a further exceptional rank-one value.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

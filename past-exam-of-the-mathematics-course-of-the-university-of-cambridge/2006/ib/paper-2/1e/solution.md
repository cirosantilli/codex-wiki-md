<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

[Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md) says that any real [quadratic form](../../../../../quadratic-form.md) has coordinates in which it is a sum of $p$ positive squares minus $m$ negative squares, with $z$ unused coordinates, and that the numbers $(p,m,z)$ are invariant under every invertible linear change of coordinates. Its [rank](../../../../../rank-one-quadratic-form.md) is $p+m$; its [signature of a quadratic form](../../../../../signature-of-a-quadratic-form.md) is commonly $p-m$, with $(p,m)$ also called its signature pair.

The [symmetric matrix](../../../../../symmetric-matrix.md) here is $J-I$, where $J=\boldsymbol1\boldsymbol1^T$ and $\boldsymbol1=(1,\ldots,1)^T$. On the line spanned by $\boldsymbol1$, $J-I$ has [eigenvalue](../../../../../eigenvalue.md) $n-1$. If $\sum_i x_i=0$, then $Jx=0$, so that the [orthogonal complement](../../../../../orthogonal-complement.md) has [eigenvalue](../../../../../eigenvalue.md) $-1$ with multiplicity $n-1$. Thus the [off-diagonal all-ones quadratic form](../../../../../off-diagonal-all-ones-quadratic-form.md) has

$$
\boxed{\operatorname{rank}q=n,\quad(p,m,z)=(1,n-1,0),\quad\sigma=2-n\qquad(n>1).}
$$

For $n=1$ the form vanishes, so **[rank](../../../../../rank-one-quadratic-form.md) and scalar signature are both zero**, with inertia $(0,0,1)$. Including this case is necessary because the distinguished [eigenvalue](../../../../../eigenvalue.md) then becomes zero.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

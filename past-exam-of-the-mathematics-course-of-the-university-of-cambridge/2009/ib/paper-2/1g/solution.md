<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

The [monomials](../../../../../monomial.md) $x^iy^j$ with $i,j\ge0$ and $i+j\le n$ form a [basis](../../../../../basis.md) of the given [vector space](../../../../../vector-space-split.md). There are $k+1$ of [total degree](../../../../../total-degree-of-a-polynomial.md) $k$, so

$$
\boxed{\dim V=\sum_{k=0}^n(k+1)=\frac{(n+1)(n+2)}2.}
$$

On that [basis](../../../../../basis.md) the [linear operator](../../../../../linear-operator.md) is diagonal:

$$
S(x^iy^j)=\bigl(i(i-1)+j(j-1)\bigr)x^iy^j.
$$

Both summands of the [eigenvalue](../../../../../eigenvalue.md) are nonnegative integers. Their sum is zero precisely when $i,j\in\{0,1\}$. Thus **the [kernel](../../../../../kernel-of-a-linear-map.md) is the span of those members of $1,x,y,xy$ whose [total degree](../../../../../total-degree-of-a-polynomial.md) is at most $n$**. In particular it is $\operatorname{span}\{1,x,y\}$ for $n=1$ and $\operatorname{span}\{1,x,y,xy\}$ for $n\ge2$; for $n=0$ it is the constants. **The [image of a linear map](../../../../../image-of-a-linear-map.md) is the span of all the other permitted [monomials](../../../../../monomial.md)**, since each has a nonzero diagonal [eigenvalue](../../../../../eigenvalue.md) and hence is the image of its reciprocal multiple. No excluded [monomial](../../../../../monomial.md) can occur in an image because its diagonal coefficient is zero.

The [trace](../../../../../matrix-trace.md) is the sum of these [eigenvalues](../../../../../eigenvalue.md). At degrees zero and one all contributions vanish. At degree two the contributions are $2,0,2$, summing to four; at degree three they are $6,2,2,6$, summing to sixteen; at degree four they are $12,6,4,6,12$, summing to forty. Therefore

$$
\boxed{\operatorname{tr}S=0,4,20,60\quad\text{for }n=1,2,3,4\text{ respectively}.}
$$

This is the [diagonal monomial action of a second-order Euler operator](../../../../../diagonal-monomial-action-of-a-second-order-euler-operator.md).

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

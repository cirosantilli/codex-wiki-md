<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a finite collection $\mathcal L$ of distinct [affine lines in a vector space](../../../../../affine-line-in-a-vector-space.md) in $\mathbb R^n$, $n\ge2$, a [joint](../../../../../joint-of-a-line-collection.md) is a point incident to $n$ lines whose direction vectors are [linearly independent](../../../../../linear-independence.md). The [joints theorem](../../../../../joints-theorem.md) asserts

$$
\boxed{\#J(\mathcal L)\lesssim_n(\#\mathcal L)^{n/(n-1)}.}
$$

In the customary three-dimensional formulation this is **$\#J\lesssim L^{3/2}$**, with three noncoplanar incident lines at every [joint](../../../../../joint-of-a-line-collection.md). We prove the general form, which includes that formulation.

Let $L=\#\mathcal L$ and $M=\#J$. The conclusion is immediate when $M=0$. Otherwise set $D=\lceil nM^{1/n}\rceil$. Suppose for contradiction that $M>LD$. Repeatedly delete any line incident to at most $D$ of the currently retained [joints](../../../../../joint-of-a-line-collection.md), deleting those [joints](../../../../../joint-of-a-line-collection.md) at the same time. Each deleted line loses at most $D$ current [joints](../../../../../joint-of-a-line-collection.md), so even deleting all $L$ lines could lose at most $LD<M$ [joints](../../../../../joint-of-a-line-collection.md). Therefore the process must stop with a nonempty set $J'$ and a line collection $\mathcal L'$ such that **each retained line contains more than $D$ retained [joints](../../../../../joint-of-a-line-collection.md)**. Every retained [joint](../../../../../joint-of-a-line-collection.md) still has its original $n$ independent incident lines: if any line through it had been deleted, the [joint](../../../../../joint-of-a-line-collection.md) would have been deleted too.

There is a nonzero [multivariate polynomial](../../../../../multivariate-polynomial.md) of [total degree](../../../../../total-degree-of-a-polynomial.md) at most $D$ vanishing on $J'$, because

$$
\binom{D+n}{n}\ge\frac{D^n}{n!}
\ge\frac{n^n}{n!}M>M\ge\#J'.
$$

Choose such a [polynomial](../../../../../polynomial-split.md) $P$ of smallest possible [total degree](../../../../../total-degree-of-a-polynomial.md) $d\le D$. This is an application of the [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md). Every line of $\mathcal L'$ contains more than $D\ge d$ [roots of a polynomial](../../../../../root-of-a-polynomial.md) of its [polynomial restriction to a line](../../../../../polynomial-restriction-to-a-line.md), so $P$ vanishes identically on every such line.

At a retained [joint](../../../../../joint-of-a-line-collection.md) $x$, differentiating along each of its independent line directions $v_1,\ldots,v_n$ gives $v_i\cdot\nabla P(x)=0$. Their [linear independence](../../../../../linear-independence.md) therefore forces $\nabla P(x)=0$. Each [partial derivative](../../../../../partial-derivative.md) of $P$ vanishes on all of $J'$ and has smaller [total degree](../../../../../total-degree-of-a-polynomial.md). Minimality of $d$ forces every [partial derivative](../../../../../partial-derivative.md) to be the zero [polynomial](../../../../../polynomial-split.md). Over the real numbers, a [polynomial](../../../../../polynomial-split.md) with all [partial derivatives](../../../../../partial-derivative.md) zero is constant; a nonzero constant cannot vanish on the nonempty $J'$. This is the required contradiction.

It follows that $M\le LD$. Since $D\le(n+1)M^{1/n}$ for $M\ge1$,

$$
M^{(n-1)/n}\le(n+1)L,
\qquad
\boxed{M\le((n+1)L)^{n/(n-1)}.}
$$

This proves the [joints theorem](../../../../../joints-theorem.md) by the [pruning and minimal-degree polynomial argument](../../../../../pruning-and-minimal-degree-polynomial-argument.md).

The exponent is sharp. Take all axis-parallel lines passing through the grid $\{1,\ldots,m\}^n$. There are $n m^{n-1}$ distinct lines and $m^n$ [joints](../../../../../joint-of-a-line-collection.md); the coordinate directions span $\mathbb R^n$ at every grid point. Thus no smaller power of the number of lines can bound all [joint](../../../../../joint-of-a-line-collection.md) configurations.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

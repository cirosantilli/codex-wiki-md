<h1 id="9g/solution">Solution</h1>

↑ **Parent:** [9G](../9g.md)

[Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md) states that a real [quadratic form](../../../../../quadratic-form.md) can be brought by an invertible real change of coordinates to

$$
Q=\sum_{j=1}^p u_j^2-\sum_{j=p+1}^{p+q}u_j^2,
$$

with $r$ remaining zero coordinates, and that the integers $(p,q,r)$ are uniquely determined. To prove existence, represent it by a [symmetric matrix](../../../../../symmetric-matrix.md). The allowed orthogonal [diagonalization](../../../../../diagonalization-of-a-matrix.md) yields real [eigenvalues](../../../../../eigenvalue.md), and scaling each nonzero eigen-coordinate by the square root of its absolute [eigenvalue](../../../../../eigenvalue.md) changes its coefficient to $+1$ or $-1$.

For uniqueness, $p$ is the largest [dimension](../../../../../dimension-vector-space.md) of a subspace on which the form is positive definite. The positive coordinate subspace attains $p$. Any subspace of [dimension](../../../../../dimension-vector-space.md) greater than $p$ intersects the $(q+r)$-dimensional span of the negative and zero coordinates nontrivially, by the [dimension](../../../../../dimension-vector-space.md) formula. A nonzero vector in that intersection has nonpositive quadratic value, contradicting positive definiteness. Similarly, $q$ is the maximal [dimension](../../../../../dimension-vector-space.md) of a negative-definite subspace. These descriptions are independent of coordinates, and $r=\dim V-p-q$ is then fixed. This proves existence and uniqueness, including degenerate forms.

For the final application, nonsingularity gives $p+q=2m$. In diagonal coordinates write $v=(v_+,v_-)$, with $Q(v)=|v_+|^2-|v_-|^2$. If $v\in U$ projects to zero in the positive coordinates, $Q(v)=0$ forces $v_-=0$, so projection $U\to\mathbb R^p$ is injective. The same argument applies to the negative coordinates. Hence $m\leq p$ and $m\leq q$, and their sum is $2m$. Therefore

$$
\boxed{p=q=m.}
$$

The inertia signature is $(m,m)$, or signature difference $p-q=0$ if that convention is used. This is the [isotropic dimension bound from real inertia](../../../../../isotropic-dimension-bound-from-real-inertia.md).

## ↑ Ancestors (10)

1. [9G](../9g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

The symmetric bilinear form associated with a real [quadratic form](../../../../../quadratic-form.md) $Q$ is obtained by [polarization identity](../../../../../polarization-identity.md):

$$
phi(u,v)=\frac12\bigl(Q(u+v)-Q(u)-Q(v)\bigr).
$$

In coordinates $Q(x)=x^TAx$, replacing $A$ by its symmetric part does not change $Q$, and the formula gives $phi(u,v)=u^TAv$; this proves existence. A symmetric form is positive semidefinite when $phi(v,v)\geq0$ for every $v$, and positive definite when the inequality is strict for every $v\ne0$.

The diagonalization theorem for real quadratic forms says that some [basis](../../../../../basis.md) puts any symmetric form into

$$
x_1^2+\cdots+x_p^2-y_1^2-\cdots-y_q^2,
$$

with $r$ further zero coordinates. [Sylvester's law of inertia](../../../../../sylvester-s-law-of-inertia.md) says that $(p,q,r)$ is independent of the diagonalizing [basis](../../../../../basis.md). To prove this, let $P$ be the span of the positive coordinate [vectors](../../../../../vector.md) and let $N\oplus Z$ be the span of the negative and zero [vectors](../../../../../vector.md). If $P'$ is positive definite for another diagonalization and $\dim P'>p$, then

$$
\dim P'+\dim(N\oplus Z)>(p+q+r),
$$

so the two spaces intersect nontrivially. A [vector](../../../../../vector.md) in the intersection would have both positive and nonpositive square, a contradiction. Thus $p'\leq p$; symmetry gives $p=p'$. Applying the same argument to $-\phi$ gives $q=q'$, and then $r=r'$.

For the [nondegenerate form](../../../../../nondegenerate-bilinear-form.md) on $V$, write its [inertia](../../../../../inertia-of-a-bilinear-form.md) as $(p,q,0)$, so $p+q=2n$. The restriction vanishes identically on $E$: [polarization](../../../../../polarization-identity.md) gives $phi(u,v)=0$ for $u,v\in E$. Projection of $E$ to the positive coordinate space is [injective](../../../../../injective-function.md), since a [vector](../../../../../vector.md) with zero positive projection cannot be [isotropic](../../../../../isotropic-vector.md) unless it is zero. Hence $k\leq p$; projection to the negative space likewise gives $k\leq q$. Therefore $k\leq\min(p,q)\leq n$.

The [matrix](../../../../../matrix.md) of $l^2$ is $ll^T$. If $l\ne0$, it has rank one and inertia $(1,0,n-1)$, hence signature one; if $l=0$, its rank and signature are zero. The coefficientwise product $(l^2,s^2)$ has [matrix](../../../../../matrix.md) $tt^T$, where $t_i=l_is_i$, so it has the same rank-one conclusion when $t\ne0$ and is zero otherwise.

Finally, diagonalization writes every positive semidefinite form as a sum of squares, say $f=\sum_a l_a^2$ and $g=\sum_b s_b^2$. Bilinearity of coefficientwise multiplication gives

$$
 (f,g)=\sum_{a,b}(l_a^2,s_b^2),
$$

a sum of positive semidefinite rank-at-most-one forms. Thus $(f,g)$ is positive semidefinite.

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

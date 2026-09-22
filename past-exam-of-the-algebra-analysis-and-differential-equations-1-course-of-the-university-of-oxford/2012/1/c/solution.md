<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [linear functional](../../../../linear-functional.md) $\lambda\in V'$, the definition of the [dual map](../../../../transpose-of-a-linear-map.md) gives

$$
\lambda\in\ker T'
\iff \lambda(Tu)=0\text{ for every }u\in U
\iff \lambda|_{\operatorname{im}T}=0.
$$

Thus the [kernel of a linear map](../../../../kernel-of-a-linear-map-split.md) is precisely the [annihilator of a vector subspace](../../../../annihilator-of-a-vector-subspace.md)

$$
\boxed{\ker T'=(\operatorname{im}T)^0.}
$$

Write $n=\dim U$, $m=\dim V$ and $r=\dim\operatorname{im}T$. The [rank-nullity theorem](../../../../rank-nullity-theorem.md), the [dimension](../../../../dimension-vector-space.md) formula for an [annihilator of a vector subspace](../../../../annihilator-of-a-vector-subspace.md), and $\dim V'=m$ give

$$
\dim\operatorname{im}T'=m-\dim\ker T'=m-(m-r)=r.
$$

Applying the same [dimension](../../../../dimension-vector-space.md) formula in $U$ gives

$$
\dim(\ker T)^0=n-\dim\ker T=r.
$$

Finally, if $\alpha=T'\lambda$ and $u\in\ker T$, then $\alpha(u)=\lambda(Tu)=\lambda(0)=0$. Therefore $\operatorname{im}T'\subseteq(\ker T)^0$. These are finite-dimensional [vector subspaces](../../../../vector-subspace.md) of equal [dimension](../../../../dimension-vector-space.md), so inclusion is equality:

$$
\boxed{\dim\operatorname{im}T'=\dim(\ker T)^0,\qquad
\operatorname{im}T'=(\ker T)^0.}
$$

This is the [dual image and kernel annihilator identity](../../../../dual-image-and-kernel-annihilator-identity.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

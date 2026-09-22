<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $V^*=V'$ for the [dual space](../../../dual-space-split.md). Define $\theta(v)(f)=f(v)$. For fixed $v$, this is a [linear functional](../../../linear-functional.md) on $V^*$; evaluation is also [linear](../../../linearity.md) in $v$, so $\theta:V\to V^{**}$ is a [linear map](../../../linear-map.md). If $v\ne0$, extend $v$ to a [basis](../../../basis.md) and take its first coordinate [linear functional](../../../linear-functional.md) $f$; then $f(v)=1$. Thus $\theta$ is [injective](../../../injective-function.md). A [dual basis](../../../dual-basis.md) has the same number of elements as the original [basis](../../../basis.md), so $\dim V=\dim V^*=\dim V^{**}$. The [rank-nullity theorem](../../../rank-nullity-theorem.md) now makes $\theta$ an [linear isomorphism](../../../linear-isomorphism.md).

The [annihilator of a vector subspace](../../../annihilator-of-a-vector-subspace.md) of a [linear subspace](../../../vector-subspace.md) $U\le V$ is

$$
U^\circ=\{f\in V^*: f(u)=0\text{ for every }u\in U\}.
$$

Extend a [basis](../../../basis.md) $v_1,\ldots,v_k$ of $U$ to a [basis](../../../basis.md) $v_1,\ldots,v_n$ of $V$, with [dual basis](../../../dual-basis.md) $f_1,\ldots,f_n$. A [linear functional](../../../linear-functional.md) belongs to $U^\circ$ exactly when its first $k$ coordinates in this [dual basis](../../../dual-basis.md) vanish. Hence $U^\circ$ has [basis](../../../basis.md) $f_{k+1},\ldots,f_n$, proving

$$
\boxed{\dim U+\dim U^\circ=\dim V.}
$$

The [dual map](../../../transpose-of-a-linear-map.md) is $\alpha^*(h)=h\circ\alpha$; here this is the algebraic [dual map](../../../transpose-of-a-linear-map.md), denoted $\alpha'$ in the source. If $v\in\ker\alpha$, then $(\alpha'h)(v)=h(\alpha v)=0$. Consequently $\operatorname{im}\alpha'\subseteq(\ker\alpha)^\circ$. Moreover,

$$
\theta(v)\in(\operatorname{im}\alpha')^\circ
\iff h(\alpha v)=0\text{ for every }h\in W^*
\iff\alpha v=0,
$$

because coordinate [linear functionals](../../../linear-functional.md) separate [vectors](../../../vector.md). This proves $(\operatorname{im}\alpha')^\circ=\theta(\ker\alpha)$, including the requested second inclusion. Taking [dimensions](../../../dimension-vector-space.md) gives

$$
\dim\operatorname{im}\alpha'=\dim V-\dim\ker\alpha=\dim\operatorname{im}\alpha.
$$

The first inclusion has equal [dimensions](../../../dimension-vector-space.md) on both sides, so

$$
\boxed{\operatorname{im}\alpha'=(\ker\alpha)^\circ,\qquad
(\operatorname{im}\alpha')^\circ=\theta(\ker\alpha).}
$$

For a [matrix](../../../matrix.md) $A=(a_{ij})$ representing $\alpha$, the matrix of $\alpha'$ in the corresponding [dual bases](../../../dual-basis.md) is $A^{\mathsf T}$: its $ji$ entry is $h_i(\alpha v_j)=a_{ij}$. Thus the [column rank](../../../column-rank.md) of $A^{\mathsf T}$ is the [row rank](../../../row-rank.md) of $A$, while the [column rank](../../../column-rank.md) of $A$ is $\dim\operatorname{im}\alpha$. Applying the established equality to these two [linear maps](../../../linear-map.md) proves **row rank equals column rank** over every [field](../../../field.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

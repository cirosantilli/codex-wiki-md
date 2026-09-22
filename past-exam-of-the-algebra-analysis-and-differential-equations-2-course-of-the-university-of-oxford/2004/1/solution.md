<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [dual basis](../../../dual-basis.md) is $E^*=\{e_1^*,\ldots,e_n^*\}$, where $e_i^*(e_j)=\delta_{ij}$ and each coordinate [linear functional](../../../linear-functional.md) extends linearly. Thus $e_i^*(\sum_j a_je_j)=a_i$. These functionals are a [basis](../../../basis.md) of $V^*$ because a [linear functional](../../../linear-functional.md) is uniquely determined by its values on $E$.

For a [linear subspace](../../../vector-subspace.md) $U$ of dimension $k$, extend a [basis](../../../basis.md) $u_1,\ldots,u_k$ to one of $V$. In its [dual basis](../../../dual-basis.md), the [annihilator of a vector subspace](../../../annihilator-of-a-vector-subspace.md) $U^\circ$ is spanned by the last $n-k$ coordinate functionals. Hence $\boxed{\dim U+\dim U^\circ=\dim V}$.

The [transpose](../../../transpose.md) in the source is the algebraic [dual map](../../../transpose-of-a-linear-map.md) $T^*:V^*\to V^*$ defined by $T^*f=f\circ T$. Composition of [linear maps](../../../linear-map.md) is linear, so $T^*f$ is a [linear functional](../../../linear-functional.md); and $T^*(af+bg)=aT^*f+bT^*g$, proving linearity in its input. If $T(e_j)=\sum_i a_{ij}e_i$, then

$$
(T^*e_i^*)(e_j)=e_i^*(Te_j)=a_{ij}.
$$

The coefficient of $e_j^*$ in $T^*e_i^*$ is consequently $a_{ij}$, so $\boxed{[T^*]_{E^*}=([T]_E)^{\mathsf T}}$. No [inner product](../../../inner-product-split.md) is involved.

A [linear functional](../../../linear-functional.md) $f$ annihilates $\operatorname{Im}T$ exactly when $f(Tv)=0$ for all $v$, equivalently $T^*f=0$. Thus $(\operatorname{Im}T)^\circ=\ker T^*$. If $v\in\ker T$, then $(T^*f)(v)=f(Tv)=0$, giving $\operatorname{Im}T^*\subseteq(\ker T)^\circ$. The first equality and the dimension formula give $\dim\ker T^*=n-\dim\operatorname{Im}T$. By the [rank-nullity theorem](../../../rank-nullity-theorem.md),

$$
\dim\operatorname{Im}T^*=\dim\operatorname{Im}T
=n-\dim\ker T=\dim(\ker T)^\circ.
$$

The inclusion is therefore an equality:

$$
\boxed{\operatorname{Im}T^*=(\ker T)^\circ.}
$$

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2004](../../2004-split.md)
3. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations II course of the University of Oxford](../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)

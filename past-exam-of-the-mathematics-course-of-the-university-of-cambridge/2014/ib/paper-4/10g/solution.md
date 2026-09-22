<h1 id="10g/solution">Solution</h1>

↑ **Parent:** [10G](../10g.md)

The algebraic [dual space](../../../../../dual-space.md) is $V^*=\operatorname{Hom}_{\mathbb R}(V,\mathbb R)$, the [vector space](../../../../../vector-space-split.md) of all real [linear functionals](../../../../../linear-functional.md). For a finite [basis](../../../../../basis.md) $e_1,\ldots,e_n$, define the [dual basis](../../../../../dual-basis.md) by $e_i^*(\sum_j a_je_j)=a_i$, so $e_i^*(e_j)=\delta_{ij}$. Every [linear functional](../../../../../linear-functional.md) satisfies

$$
 \lambda=\sum_{i=1}^n\lambda(e_i)e_i^*.
$$

This equality follows by evaluating both sides on each vector of the [basis](../../../../../basis.md). It proves spanning directly. If $\sum_i b_ie_i^*=0$, evaluation on $e_j$ gives $b_j=0$, proving linear independence without assuming a theorem on dual dimensions.

For a [vector subspace](../../../../../vector-subspace.md) $U$, its [annihilator of a vector subspace](../../../../../annihilator-of-a-vector-subspace.md) is

$$
 U^\circ=\{\lambda\in V^*: \lambda(u)=0\text{ for all }u\in U\}.
$$

Extend a [basis](../../../../../basis.md) $e_1,\ldots,e_r$ of $U$ to a [basis](../../../../../basis.md) of $V$. Then $U^\circ$ has [basis](../../../../../basis.md) $e_{r+1}^*,\ldots,e_n^*$, so $\boxed{\dim U^\circ=n-\dim U}$.

The [dual map](../../../../../transpose-of-a-linear-map.md) of $\alpha:V\to W$ is $\alpha^*:W^*\to V^*$, $\lambda\mapsto\lambda\circ\alpha$. In the corresponding [dual bases](../../../../../dual-basis.md) its [matrix](../../../../../matrix.md) is the transpose of the [matrix](../../../../../matrix.md) for $\alpha$. A [matrix](../../../../../matrix.md) and its transpose have the same [rank](../../../../../rank-one-quadratic-form.md), giving $\operatorname{rank}\alpha^*=\operatorname{rank}\alpha$. Directly,

$$
 \alpha^*\lambda=0\ \Longleftrightarrow\ \lambda(\alpha v)=0\text{ for all }v
 \ \Longleftrightarrow\ \lambda\in(\operatorname{im}\alpha)^\circ.
$$

Thus $\boxed{\ker\alpha^*=(\operatorname{im}\alpha)^\circ}$. Also every $\lambda\circ\alpha$ vanishes on $\ker\alpha$, so $\operatorname{im}\alpha^*\subseteq(\ker\alpha)^\circ$. Both spaces have dimension $\operatorname{rank}\alpha$ by the preceding [annihilator of a vector subspace](../../../../../annihilator-of-a-vector-subspace.md) formula and [rank-nullity theorem](../../../../../rank-nullity-theorem.md), proving

$$
 \boxed{\operatorname{im}\alpha^*=(\ker\alpha)^\circ.}
$$

Alternatively, a [linear functional](../../../../../linear-functional.md) vanishing on the kernel descends to the image of $\alpha$ and can be extended to $W$ by extending a [basis](../../../../../basis.md).

For the infinite-dimensional [polynomial ring](../../../../../polynomial-ring.md), the coefficient functionals $L_i$ are linearly independent: evaluate a finite relation on each monomial. However, they do not span the algebraic [dual space](../../../../../dual-space.md). The [linear functional](../../../../../linear-functional.md) $p\mapsto p(1)$ takes value one on every monomial, while any finite combination of the $L_i$ vanishes on every sufficiently high-degree monomial. Thus **the $L_i$ do not form a basis of $V^*$**. An infinite formal sum of coefficient functionals is not a finite linear combination.

## ↑ Ancestors (10)

1. [10G](../10g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

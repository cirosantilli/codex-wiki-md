<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) says that for a [linear map](../../../../../linear-map.md) $T:V\to W$ with finite-dimensional [domain of a function](../../../../../domain-of-a-function.md) $V$,

$$
\boxed{\dim V=\dim\ker T+\dim\operatorname{im}T=\operatorname{nullity}T+\operatorname{rank}T.}
$$

Take a [basis](../../../../../basis.md) $k_1,\ldots,k_r$ of the [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) and use [basis extension](../../../../../basis-extension.md) to obtain a [basis](../../../../../basis.md) $k_1,\ldots,k_r,u_1,\ldots,u_s$ of $V$. We show that $T(u_1),\ldots,T(u_s)$ is a [basis](../../../../../basis.md) of the [image of a linear map](../../../../../image-of-a-linear-map.md).

Every $v\in V$ is a [linear combination](../../../../../linear-combination.md) of the extended [basis](../../../../../basis.md), and its $k_i$ terms vanish under $T$. Therefore $T(v)$ is a [linear combination](../../../../../linear-combination.md) of the $T(u_j)$, proving the required [linear span](../../../../../linear-span.md) property. For [linear independence](../../../../../linear-independence.md), suppose $\sum_j b_jT(u_j)=0$. Then $\sum_j b_ju_j\in\ker T$, so $\sum_j b_ju_j=\sum_i a_ik_i$ for some real [scalars](../../../../../scalar.md) $a_i$. The extended [basis](../../../../../basis.md) is [linearly independent](../../../../../linear-independence.md), forcing every $a_i$ and $b_j$ to be zero. Thus the [image of a linear map](../../../../../image-of-a-linear-map.md) has [dimension](../../../../../dimension-vector-space.md) $s$, the [kernel of a linear map](../../../../../kernel-of-a-linear-map-split.md) has [dimension](../../../../../dimension-vector-space.md) $r$, and $\dim V=r+s$ proves the result.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)

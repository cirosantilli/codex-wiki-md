<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [rank-nullity theorem](../../../../../../rank-nullity-theorem.md) states that a [linear map](../../../../../../linear-map.md) $T:V\to W$ with finite-dimensional $V$ satisfies

$$
\boxed{\dim V=\operatorname{nullity}T+\operatorname{rank}T.}
$$

Choose a [basis](../../../../../../basis.md) $k_1,\ldots,k_r$ of $\ker T$ and use [basis extension](../../../../../../basis-extension.md) to obtain a [basis](../../../../../../basis.md) $k_1,\ldots,k_r,u_1,\ldots,u_s$ of $V$. We prove that $Tu_1,\ldots,Tu_s$ is a [basis](../../../../../../basis.md) of $\operatorname{im}T$.

Every $v\in V$ is a [linear combination](../../../../../../linear-combination.md) of the extended [basis](../../../../../../basis.md). Applying $T$ kills the $k_i$ terms, so $Tv$ is a [linear combination](../../../../../../linear-combination.md) of $Tu_1,\ldots,Tu_s$. This proves the [linear span](../../../../../../linear-span.md) assertion. For [linear independence](../../../../../../linear-independence.md), if $\sum_j b_jTu_j=0$, then $\sum_j b_ju_j$ belongs to the [kernel of a linear map](../../../../../../kernel-of-a-linear-map-split.md). Hence $\sum_j b_ju_j=\sum_i a_ik_i$ for some [scalars](../../../../../../scalar.md) $a_i$. The [linear independence](../../../../../../linear-independence.md) of the extended [basis](../../../../../../basis.md) forces every $a_i$ and $b_j$ to vanish. Consequently $\operatorname{rank}T=s$ and $\operatorname{nullity}T=r$, while $\dim V=r+s$, proving the theorem.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Calculus, probability, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../../calculus-probability-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
5. [2003](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)

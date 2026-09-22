<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

Every finite [cyclic subgroup](../../../../../cyclic-subgroup.md) of order $m$ has exactly $\varphi(m)$ generators, where $\varphi$ is the [Euler totient function](../../../../../euler-totient-function.md): if $g$ has order $m$, then $g^k$ generates precisely when $\gcd(k,m)=1$. Each element generates exactly one [cyclic subgroup](../../../../../cyclic-subgroup.md). Thus [counting cyclic subgroups by their generators](../../../../../counting-cyclic-subgroups-by-their-generators.md) amounts to counting elements by [order of a group element](../../../../../order-of-a-group-element.md) and dividing by $\varphi(m)$.

Use the [cycle decomposition of a permutation](../../../../../cycle-decomposition-of-a-permutation.md) in $S_5$. A [permutation](../../../../../permutation.md) with $a_j$ cycles of length $j$ occurs $5!/\prod_j(j^{a_j}a_j!)$ times: order the five letters, then divide by the cyclic choices of starting point and the orderings of equal-length cycles. Its order is the [least common multiple](../../../../../least-common-multiple.md) of the cycle lengths. The resulting count is

$$
\begin{array}{c|r|r|r}
\text{cycle type}&\text{elements}&\text{order}&\text{cyclic subgroups}\\\hline
1^5&1&1&1\\
2\,1^3&10&2&10\\
2^2\,1&15&2&15\\
3\,1^2&20&3&10\\
3\,2&20&6&10\\
4\,1&30&4&15\\
5&24&5&6
\end{array}
\qquad \boxed{1+10+15+10+10+15+6=67.}
$$

The two [subgroups](../../../../../subgroup.md) $\langle(12)\rangle$ and $\langle(12)(34)\rangle$ are both isomorphic to $C_2$ by a [group isomorphism](../../../../../group-isomorphism.md). They are not [conjugate subgroups](../../../../../conjugate-subgroup.md): conjugating their unique nonidentity elements would have to preserve [cycle type](../../../../../cycle-type.md), whereas a transposition and a product of two disjoint transpositions have different [cycle types](../../../../../cycle-type.md).

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

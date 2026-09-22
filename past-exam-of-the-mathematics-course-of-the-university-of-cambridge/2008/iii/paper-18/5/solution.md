<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For closed connected oriented $d$-manifolds, the [degree of a map between oriented manifolds](../../../../../degree-of-a-map-between-oriented-manifolds.md) is the integer defined by $f_*[M]=(\deg f)[N]$ in $H_d(N;\mathbb Z)$. If $y\in N$ has finite fiber $\{x_1,\ldots,x_r\}$, choose disjoint small neighbourhoods $U_i$ containing no other points of that fiber. The map of local [relative homology](../../../../../relative-homology.md) groups

$$
H_d(U_i,U_i\setminus\{x_i\};\mathbb Z)\longrightarrow H_d(N,N\setminus\{y\};\mathbb Z)
$$

sends the local orientation generator at $x_i$ to $d_i$ times the one at $y$. This integer is its [local degree of a continuous map](../../../../../local-degree-of-a-continuous-map.md), independent of the small neighbourhood by [excision](../../../../../excision-theorem.md). Excision also identifies $H_d(M,M\setminus f^{-1}(y))$ with the direct sum of the local groups, and the global fundamental class restricts to their orientation generators. Naturality of the maps to relative homology therefore proves the [degree as a sum of local degrees](../../../../../degree-as-a-sum-of-local-degrees.md):

$$
\boxed{\deg f=\sum_{i=1}^r\deg_{x_i}f.}
$$

The empty fiber gives degree zero. For smooth maps at a regular value, a local degree is the sign of the derivative determinant, but general continuous maps can have larger local multiplicities.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

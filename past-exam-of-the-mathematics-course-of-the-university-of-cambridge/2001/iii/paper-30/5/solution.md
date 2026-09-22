<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Code the two levels of each factor as $\pm1$. For a factor subset $A$, its [factorial contrast](../../../../../factorial-contrast.md) column is the character $\chi_A(x)=\prod_{j\in A}x_j$. Products of columns correspond to symmetric differences of subsets, because $x_j^2=1$.

Let $G_1,\ldots,G_k$ be defining words whose incidence vectors are linearly independent over $\mathbb F_2$. Write $x_j=(-1)^{u_j}$, with $u_j\in\mathbb F_2$. Specifying signs $\chi_{G_i}(x)=s_i$ is then a rank-$k$ system of binary linear equations. Every one of its $2^k$ right-hand sides has $2^{n-k}$ solutions. Thus **$k$ independent defining contrasts split the full $2^n$ design into $2^k$ equal fractions.** Independence is necessary: dependent defining words do not yield $2^k$ distinct sets.

The [defining contrast subgroup](../../../../../defining-contrast-subgroup.md) has $2^k$ words. On a selected fraction its word $G$ has a constant sign $s_G$, so

$$
\chi_{AG}=s_G\chi_A.
$$

Hence the coefficients of $A$ and $AG$ cannot be estimated separately without assumptions or extra runs: this is [aliasing in a fractional factorial design](../../../../../aliasing-in-a-fractional-factorial-design.md). Conversely, averaging a character over the affine binary solution space vanishes unless its word is in the defining subgroup, so these signed subgroup cosets give all aliases. Here a lowercase treatment label records the factors at their high levels, and $(1)$ puts all five at their low levels; signs must be retained when listing aliases.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

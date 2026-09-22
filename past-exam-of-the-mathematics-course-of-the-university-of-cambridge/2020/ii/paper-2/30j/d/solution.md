<h1 id="30j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For each $d$-element coordinate set $J\subseteq\{1,\ldots,p\}$, let $\mathcal G_J$ contain the lower orthants whose finite thresholds occur precisely in the coordinates in $J$. Ignoring the remaining coordinates identifies $\mathcal G_J$ with the lower-orthant class in $\mathbb R^d$, so part (a) gives $\operatorname{VC}(\mathcal G_J)=d$. Moreover,

$$
\mathcal G=\bigcup_{|J|=d}\mathcal G_J
$$

is a union of $r=\binom pd$ such classes. Part (c) and $\binom pd\leq p^d$ give

$$
\begin{aligned}
\operatorname{VC}(\mathcal G)
&\leq4d\log_2(2d)+2\log_2\binom pd\\
&\leq4d\log_2(2d)+2d\log_2p\\
&=\boxed{2d\{2\log_2(2d)+\log_2p\}}.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [30J](../../30j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a compatible complete metric on the [Polish space](../../../../../../polish-space.md) $P$. For a [tree on a Polish space](../../../../../../tree-on-a-polish-space.md) $T\subseteq\bigcup_nP^n$, let

$$
r_T(t)=\sup\{r_T(t^\frown x)+1:t^\frown x\in T\}
$$

be its [rank of a well-founded tree](../../../../../../rank-of-a-well-founded-tree.md), with terminal rank zero. We bound this rank using a countable approximation tree, rather than assuming that the original tree has countably many nodes.

Choose a countable base of open balls. A node of the approximation tree $S$ at depth $n$ records, for every coordinate $i\leq j\leq n$, a basic ball $U_{j,i}$. Require its diameter to be less than $2^{-j}$, require $\overline{U_{j+1,i}}\subseteq U_{j,i}$, and require

$$
T_j\cap\prod_{i=1}^jU_{j,i}\ne\varnothing\qquad(1\leq j\leq n).
$$

Initial truncation removes the last row of balls. There are only countably many such finite records, so $S$ is countable.

An infinite branch in $S$ would give, by completeness and shrinking nested balls, a limit $p_i\in P$ for each coordinate. For fixed $j$, witnesses from later levels of $T$ have their first $j$ coordinates converging to $(p_1,\ldots,p_j)$. Initial-segment closure puts those witnesses in $T_j$, and closedness of $T_j$ puts the limit there too. Hence $(p_i)$ would be an infinite branch of $T$. Thus $S$ is well-founded.

Every tuple $t=(p_1,\ldots,p_n)\in T_n$ can be fitted inside such a record with each $p_i\in U_{n,i}$. Every extension $t^\frown p$ can be fitted in a child record: shrink the old balls around their actual points and choose a small ball around the new point. A well-founded induction therefore gives $r_T(t)\leq r_S(s)$ whenever the record $s$ fits $t$. At the empty record this bounds the whole tree's rank by $r_S(\varnothing)$.

The rank of a countable well-founded tree is countable: at each node it is a supremum of countably many successors of countable ordinals, by well-founded recursion. Consequently **a closed well-founded tree on a Polish space has countable height**. The completeness and closedness assumptions are precisely what turn a branch of approximation records into an actual branch.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

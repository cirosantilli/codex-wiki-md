<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Membership follows from $\mathbf{NL}=\mathbf{co\text{-}NL}$. A directed graph is not [strongly connected](../../../../../../strong-connectivity.md) exactly when there is a pair $(u,v)$ for which $v$ is not reachable from $u$. Guessing the pair and using the NL procedure for non-reachability puts non-strong-connectivity in NL, hence strong connectivity is in co-NL and therefore in NL.

For NL-hardness, reduce directed reachability. Given $(G,s,t)$, form $G'$ by retaining all edges of $G$, adding $v\to s$ for every vertex $v$, and adding $t\to v$ for every vertex $v$. If $t$ is reachable from $s$ in $G$, then any $u$ reaches any $v$ in $G'$ along

$$
u\longrightarrow s\longrightarrow t\longrightarrow v.
$$

Conversely, if $G'$ is strongly connected then $s$ reaches $t$. A simple $s$-to-$t$ path cannot use an added edge out of $t$ before arriving at $t$, and every added edge into $s$ merely returns the path to its starting vertex; deleting the resulting cycle leaves an $s$-to-$t$ path made from edges of $G$. The construction is computable in logarithmic space, so deciding [strong connectivity](../../../../../../strong-connectivity.md) is

$$
\boxed{\mathbf{NL}\text{-complete}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

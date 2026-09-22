<h1 id="3/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The optimum radius is a distance from some city to a selected city, so it belongs to

$$
D=\{0\}\cup\{d(u,v):u,v\in V,\ u\ne v\}.
$$

Sort the distinct values of $D$, try them in increasing order, and run part (i)'s greedy procedure with each trial value $r$. Declare a trial successful when all cities are covered using at most $k$ centers; stop a failed trial as soon as a $(k+1)$st center would be selected. The trial $r=r^*$ must succeed by part (i), so the first successful value $\widehat r$ satisfies $\widehat r\leq r^*$. Its output has

$$
\boxed{R\leq2\widehat r\leq2r^*.}
$$

There are $O(n^2)$ candidate distances and $O(n^2)$ work per trial, giving a [polynomial-time algorithm](../../../../../../polynomial-time-algorithm.md) with [running time](../../../../../../running-time.md) $O(n^4)$, plus sorting. Success at $r$ need not mean that radius $r$ itself is feasible; only the radius-$2r$ guarantee is used.

A faster alternative is the [farthest-first traversal](../../../../../../farthest-first-traversal.md). Choose any first center, then repeatedly choose a city farthest from its nearest current center until $k$ have been chosen. Let $R$ be the resulting radius. If $R>0$, adjoin a city attaining that distance. At every earlier selection, the maximum distance to the then-current center [set](../../../../../../set-split.md) was at least $R$, so all pairs among these $k+1$ cities are at distance at least $R$. Two belong to the same optimal radius-$r^*$ [closed ball](../../../../../../closed-ball.md), giving $R\leq2r^*$ by the [triangle inequality](../../../../../../triangle-inequality.md). If $R=0$, the guarantee is immediate. Maintaining nearest-center distances gives **$O(nk)$ distance evaluations** without knowing $r^*$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Algorithms](../../../../algorithms-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

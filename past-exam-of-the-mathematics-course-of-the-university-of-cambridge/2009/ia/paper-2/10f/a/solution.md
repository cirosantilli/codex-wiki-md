<h1 id="10f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

View the accessible rooms as the open cluster of [bond percolation](../../../../../../bond-percolation-split.md) on a rooted ternary [tree](../../../../../../tree-graph-theory.md). Each accessible room has three forward corridors, independently open with probability $2/3$, so its number of accessible children has the [binomial distribution](../../../../../../binomial-distribution.md) $\operatorname{Bin}(3,2/3)$. The counts at successive levels form a [binomial branching process](../../../../../../binomial-branching-process.md) with offspring [probability generating function](../../../../../../probability-generating-function.md)

$$
\boxed{\phi(t)=\left(\frac13+\frac23t\right)^3.}
$$

Let $q_N$ be the probability that the root has no open path to level $N$. Then $q_0=0$, and independence of the three descendant subtrees gives

$$
q_{N+1}=\left(\frac13+\frac23q_N\right)^3=\phi(q_N).
$$

The sequence increases to the smallest fixed point $q=\phi(q)$ in $[0,1]$, the [branching extinction probability](../../../../../../extinction-probability-of-a-branching-process.md). Thus $q_N$ is close to that solution for large $N$.

Connectivity is the relevant escape event: if no window is reachable, escape is impossible; if one is reachable, ordinary random wandering reaches a window eventually with probability one. Before reaching level $N$ the guest moves within a finite connected graph, so an accessible exit cannot be avoided forever. This interpretation does not require the guest to move monotonically outward.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [10F](../../10f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

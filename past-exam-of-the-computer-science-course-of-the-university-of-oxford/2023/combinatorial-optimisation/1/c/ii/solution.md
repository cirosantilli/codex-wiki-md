<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For every $S\subseteq V$ and $x\notin S$, including $S=\varnothing$, the [marginal increment](../../../../../../marginal-increment-of-a-set-function.md) is

$$
\Delta_x f(S)=\max\{0,w(x)-f(S)\}.
$$

For the [empty set](../../../../../../empty-set.md), this uses $w(x)\geq f(\varnothing)=\min_{v\in V}w(v)$. The [monotone set function](../../../../../../monotone-set-function.md) property from (i) gives $f(A)\leq f(B)$ when $A\subseteq B$. Consequently

$$
\max\{0,w(x)-f(A)\}\geq\max\{0,w(x)-f(B)\}.
$$

Thus [diminishing returns](../../../../../../diminishing-returns-characterization-of-submodularity.md) holds, so **$f$ is a [submodular set function](../../../../../../submodular-set-function.md)** by (b).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Combinatorial optimisation](../../../../combinatorial-optimisation-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)

<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Ramsey number](../../../../../ramsey-number.md) $R(s,t)$ is the smallest integer $N$ such that every red-blue colouring of the edges of $K_N$ has a red $K_s$ or a blue $K_t$. Equivalently, every [graph](../../../../../graph-split.md) on $N$ vertices contains a [clique](../../../../../clique-graph-theory.md) of size $s$ or an [independent set](../../../../../independent-set-graph-theory.md) of size $t$.

Set $R(1,t)=R(s,1)=1$. For $s,t\geq2$, let $N=R(s-1,t)+R(s,t-1)$ and fix a [vertex](../../../../../vertex-graph-theory.md) $v$ in a red-blue colouring of $K_N$. Among the remaining $N-1$ vertices, either at least $R(s-1,t)$ are red neighbors of $v$, or at least $R(s,t-1)$ are blue neighbors. In the first case their induced colouring gives a red $K_{s-1}$, which extends with $v$ to a red $K_s$, or a blue $K_t$. The second case is symmetric. This proves the [Ramsey number recursion](../../../../../ramsey-number-recursion.md)

$$
R(s,t)\leq R(s-1,t)+R(s,t-1).
$$

[Induction](../../../../../mathematical-induction.md) on $s+t$, using the boundary values and Pascal's identity, now gives the [binomial upper bound for a Ramsey number](../../../../../binomial-upper-bound-for-a-ramsey-number.md):

$$
\begin{aligned}
R(s,t)&\leq\binom{s+t-3}{t-1}+\binom{s+t-3}{t-2}\\
&=\boxed{\binom{s+t-2}{t-1}}.
\end{aligned}
$$

In particular this [induction](../../../../../mathematical-induction.md) proves that the required [Ramsey number](../../../../../ramsey-number.md) exists.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../split.md)
6. [Graph Theory and Probabilistic Combinatorics course of the University of Oxford](../../../../../graph-theory-and-probabilistic-combinatorics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

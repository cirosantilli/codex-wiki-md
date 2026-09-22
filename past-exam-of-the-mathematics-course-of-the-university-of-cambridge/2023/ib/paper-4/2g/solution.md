<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

Fix $x\in X$. By assumption there is a neighbourhood $U$ of $x$ on which $f_n\to f$ with [uniform convergence](../../../../../uniform-convergence.md). Each restriction $f_n|_U$ is [continuous](../../../../../continuous-function.md), and a uniform limit of continuous functions is continuous. Thus $f|_U$ is continuous, in particular at $x$. Since $x$ was arbitrary, $f$ is continuous on $X$.

Now let $K\subseteq X$ be [compact](../../../../../compact-space.md) and let $\varepsilon>0$. For each $x\in K$, choose a neighbourhood $U_x$ on which convergence is uniform. The sets $U_x$ cover $K$, so compactness gives a finite subcover

$$
K\subseteq U_{x_1}\cup\cdots\cup U_{x_m}.
$$

For each $j$, choose $N_j$ such that

$$
n\geq N_j,\ y\in U_{x_j}
\quad\Longrightarrow\quad |f_n(y)-f(y)|<\varepsilon.
$$

Taking $N=\max_jN_j$, every $y\in K$ belongs to one of these finitely many neighbourhoods, and therefore

$$
n\geq N\quad\Longrightarrow\quad
\sup_{y\in K}|f_n(y)-f(y)|<\varepsilon.
$$

**Thus $f_n\to f$ uniformly on every compact subset. This proves the [local uniform convergence on compact subsets](../../../../../local-uniform-convergence-on-compact-subsets.md) principle.**

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

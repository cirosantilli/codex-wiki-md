# Robust linear optimization over the probability simplex

↑ **Parent:** [Robust optimization](robust-optimization.md)

Worst-case linear revenue over a [polyhedral uncertainty set](polyhedral-uncertainty-set.md) is optimized by the linear program

$$
\max_{x,\alpha,\beta}\ r_0^Tx-\mathbf1^T(\alpha+\beta),\qquad x\in\Delta_n,\quad\alpha,\beta\ge0,\quad P^T(\alpha-\beta)=x.
$$

Here $\Delta_n$ is the [probability simplex](probability-simplex.md). Finite decisions are exactly its intersection with $\operatorname{range}P^T$. If this intersection is empty, all decisions have worst-case value $-\infty$ and the displayed linear program is infeasible; its supremum over the empty feasible set is also $-\infty$. Full column rank of $P$ suffices to make all simplex decisions finite.

## ↑ Ancestors (6)

1. [Robust optimization](robust-optimization.md)
2. [Convex optimization](convex-optimization-split.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-339/1/b/iii/solution.md)

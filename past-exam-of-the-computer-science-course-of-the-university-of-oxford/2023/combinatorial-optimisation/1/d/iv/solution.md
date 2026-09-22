<h1 id="1/d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**With nonnegative weights, the [hypergraph cut function](../../../../../../hypergraph-cut-function.md) is a [symmetric set function](../../../../../../symmetric-set-function.md) and a [submodular set function](../../../../../../submodular-set-function.md), but need not be a [monotone set function](../../../../../../monotone-set-function.md).** The proofs of symmetry and failure of monotonicity in (i) and (ii) still apply.

For [submodularity](../../../../../../submodular-set-function.md), write $f(S)=\sum_{e\in E}w(e)q_e(S)$, where $q_e(S)$ is the [indicator function](../../../../../../indicator-function.md) that $e$ meets both sides. Fix $x\notin S$. If $x\notin e$, its [marginal increment](../../../../../../marginal-increment-of-a-set-function.md) is zero. If $x\in e$, let $m=|e|\geq2$ and $j=|S\cap(e\setminus\{x\})|$. Its [marginal increment](../../../../../../marginal-increment-of-a-set-function.md) is

$$
\Delta_x q_e(S)=
\begin{cases}
1,&j=0,\\
0,&0<j<m-1,\\
-1,&j=m-1.
\end{cases}
$$

For $m=2$, the middle case is absent. As $S$ grows without acquiring $x$, $j$ can only increase, so these [marginal increments](../../../../../../marginal-increment-of-a-set-function.md) can only decrease. Each $q_e$ therefore satisfies [diminishing returns](../../../../../../diminishing-returns-characterization-of-submodularity.md). Multiplying by $w(e)\geq0$ and summing preserves the inequality, proving [submodularity](../../../../../../submodular-set-function.md) of $f$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [D](../../d.md)
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

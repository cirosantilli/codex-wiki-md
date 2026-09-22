<h1 id="22f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The pointwise limit $f$ is a [measurable function](../../../../../../measurable-function.md), since it can be expressed as $\sup_n\inf_{m\ge n}f_m$. Thus each [set](../../../../../../set-split.md) $E_n^{(k)}$ is a countable intersection of measurable [sets](../../../../../../set-split.md) within $A$. Deleting the condition at index $m=n$ weakens the requirements, whereas replacing $1/k$ by $1/(k+1)$ strengthens them. Hence

$$
\boxed{E_n^{(k)}\subseteq E_{n+1}^{(k)},\qquad E_n^{(k+1)}\subseteq E_n^{(k)}}.
$$

These are inclusions, not necessarily strict inclusions. The displayed [sets](../../../../../../set-split.md) describe eventual uniform error tolerances at an individual point.

Fix $k\ge1$ and $x\in A$. By [pointwise convergence](../../../../../../pointwise-convergence.md), there is an $N=N(x,k)$ such that $|f_m(x)-f(x)|\le1/k$ for every $m\ge N$. This is exactly $x\in E_N^{(k)}$, proving

$$
\boxed{A=\bigcup_{n\ge1}E_n^{(k)}}.
$$

Together with monotonicity in $n$ and finite measure of $A$, [continuity from below of a measure](../../../../../../continuity-from-below-of-a-measure.md) gives $\lambda(E_n^{(k)})\uparrow\lambda(A)$. Consequently

$$
\lambda(A\setminus E_n^{(k)})\longrightarrow0.
$$

This quantitative form is what allows a single large-measure [set](../../../../../../set-split.md) to work for every tolerance, rather than choosing a different exceptional [set](../../../../../../set-split.md) for each point.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22F](../../22f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

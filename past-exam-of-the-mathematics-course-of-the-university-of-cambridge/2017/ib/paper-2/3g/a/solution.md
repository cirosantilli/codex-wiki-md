<h1 id="3g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [uniform convergence](../../../../../../uniform-convergence.md) condition on a set $X$ is

$$
\boxed{\forall\epsilon>0\ \exists N\ \forall n\ge N\ \forall x\in X:\quad |f_n(x)-f(x)|<\epsilon.}
$$

The index $N$ is independent of $x$; this is stronger than [pointwise convergence](../../../../../../pointwise-convergence.md).

Fix $x_0\in\mathbb R$ and $\epsilon>0$. Choose one $N$ such that $|f_N(x)-f(x)|<\epsilon/3$ for every $x$. The [continuity](../../../../../../continuous-function.md) of $f_N$ at $x_0$ gives $\delta>0$ with $|f_N(x)-f_N(x_0)|<\epsilon/3$ whenever $|x-x_0|<\delta$. The [triangle inequality](../../../../../../triangle-inequality.md) then gives

$$
|f(x)-f(x_0)|\le |f(x)-f_N(x)|+|f_N(x)-f_N(x_0)|+|f_N(x_0)-f(x_0)|<\epsilon.
$$

Since $x_0$ was arbitrary, $\boxed{f\text{ is continuous on }\mathbb R}$, the [uniform limit theorem](../../../../../../uniform-limit-theorem.md). Continuity of each approximant need not be uniform continuity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3G](../../3g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

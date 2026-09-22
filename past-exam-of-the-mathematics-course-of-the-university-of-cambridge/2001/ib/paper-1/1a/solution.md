<h1 id="1a/solution">Solution</h1>

↑ **Parent:** [1A](../1a.md)

A [function](../../../../../function-split.md) $f:I\to\mathbb R$ is [uniformly continuous](../../../../../uniform-continuity.md) if

$$
\forall\varepsilon>0\ \exists\delta>0\ \forall x,y\in I:\quad |x-y|<\delta\Longrightarrow|f(x)-f(y)|<\varepsilon.
$$

The crucial point is that $\delta$ works throughout the [interval](../../../../../interval-mathematics.md), not just near one chosen point.

**Yes, it is bounded on the closed unit interval.** Choose $\delta$ for $\varepsilon=1$, and choose finitely many grid points $t_j$ such that every $x\in[0,1]$ is within $\delta$ of some $t_j$. Then $|f(x)|\leq1+\max_j|f(t_j)|$, a finite bound. Equivalently, [uniform continuity](../../../../../uniform-continuity.md) implies [continuity](../../../../../continuous-function.md), and a continuous real [function](../../../../../function-split.md) on a [compact set](../../../../../compact-space.md) is bounded.

**Yes, a bounded [derivative](../../../../../derivative.md) gives [uniform continuity](../../../../../uniform-continuity.md) on the half-line.** If $|f'|\leq K$, the [mean value theorem](../../../../../mean-value-theorem.md) gives $|f(x)-f(y)|\leq K|x-y|$. This is a [Lipschitz condition](../../../../../lipschitz-continuity.md), so for $K>0$ use $\delta=\varepsilon/K$. If $K=0$, the [function](../../../../../function-split.md) is constant. As usual for a [derivative](../../../../../derivative.md) on this closed half-line, [continuity](../../../../../continuous-function.md) at its endpoint is included.

## ↑ Ancestors (10)

1. [1A](../1a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

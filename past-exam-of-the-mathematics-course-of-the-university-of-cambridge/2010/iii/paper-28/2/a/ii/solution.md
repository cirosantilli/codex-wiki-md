<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each positive integer $m$, apply part (i) to the grid $D_m=\{j/m:0\leq j\leq m\}$. Intersect the resulting probability-one events over all $m$, a countable intersection. Work on this common event.

For $x\in[j/m,(j+1)/m]$, monotonicity of the [empirical distribution function](../../../../../../../empirical-distribution-function.md) gives $F_n(j/m)\leq F_n(x)\leq F_n((j+1)/m)$. Consequently

$$
F_n(x)-x\leq F_n((j+1)/m)-(j+1)/m+1/m,
$$

and

$$
x-F_n(x)\leq j/m-F_n(j/m)+1/m.
$$

The endpoint $x=1$ is itself on the grid. Therefore

$$
\sup_{x\in[0,1]}|F_n(x)-x|
\leq\max_{t\in D_m}|F_n(t)-t|+\frac1m.
$$

For each fixed $m$, take the upper limit as $n\to\infty$; part (i) makes the maximum vanish. Then let $m\to\infty$. This proves

$$
\boxed{\sup_{x\in[0,1]}|F_n(x)-x|\longrightarrow0\quad\text{almost surely}.}
$$

This is the uniform-sample case of the [Glivenko-Cantelli theorem](../../../../../../../glivenko-cantelli-theorem.md), proved by a finite-grid approximation rather than assumed.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [Paper 28](../../../../paper-28-split.md)
5. [Iii](../../../../split.md)
6. [2010](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

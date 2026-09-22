<h1 id="3e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A sequence of functions $f_n:A\to\mathbb R$ [converges uniformly](../../../../../../uniform-convergence.md) to $f$ when, for every $\varepsilon>0$, there is an $N$ such that

$$
n\geq N\quad\Longrightarrow\quad |f_n(x)-f(x)|<\varepsilon
$$

for every $x\in A$. Equivalently, $\lVert f_n-f\rVert_\infty\to0$ in the [supremum norm](../../../../../../supremum-norm.md).

**Yes.** Fix $x_0\in A$ and $\varepsilon>0$. Uniform convergence gives $N$ such that $|f_N(x)-f(x)|<\varepsilon/3$ for every $x\in A$. Since the [continuous function](../../../../../../continuous-function.md) $f_N$ is continuous at $x_0$, there is a $\delta>0$ such that $|x-x_0|<\delta$ implies $|f_N(x)-f_N(x_0)|<\varepsilon/3$. The [triangle inequality](../../../../../../triangle-inequality.md) then gives

$$
|f(x)-f(x_0)|
\leq |f(x)-f_N(x)|+|f_N(x)-f_N(x_0)|+|f_N(x_0)-f(x_0)|
<\varepsilon.
$$

This proves the [uniform limit theorem](../../../../../../uniform-limit-theorem.md): $f$ is continuous.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3E](../../3e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

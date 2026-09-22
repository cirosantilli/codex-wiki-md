<h1 id="12g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose the continuous $f$ were not [uniformly continuous](../../../../../../uniform-continuity.md). There would be an $\varepsilon_0>0$ and pairs $x_n,y_n\in X$ with $d(x_n,y_n)<1/n$ but $|f(x_n)-f(y_n)|\geq\varepsilon_0$. [Sequential compactness](../../../../../../sequentially-compact-space.md) gives a subsequence $x_{n_j}\to x\in X$. The [triangle inequality](../../../../../../triangle-inequality.md) gives $y_{n_j}\to x$ as well. [Continuity](../../../../../../continuous-function.md) at $x$ then gives $f(x_{n_j})-f(y_{n_j})\to0$, a contradiction. Thus **$f$ is uniformly continuous**.

It need not be [Lipschitz continuous](../../../../../../lipschitz-continuity.md). On the sequentially compact interval $[0,1]$, the continuous function $f(x)=\sqrt x$ has

$$
\frac{|f(x)-f(0)|}{|x-0|}=\frac1{\sqrt x}\to\infty\quad(x\downarrow0).
$$

No finite Lipschitz constant exists.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12G](../../12g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

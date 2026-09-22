<h1 id="12g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Nonnegativity and symmetry are immediate. Moreover, $d(x,y)=0$ exactly when $n_{\min}(x,y)=\infty$, which means $x_n=y_n$ for every $n$.

For three sequences $x,y,z$, if $x$ and $y$ agree through coordinate $r-1$ and $y$ and $z$ agree through coordinate $s-1$, then $x$ and $z$ agree through coordinate $\min(r,s)-1$. Hence

$$
n_{\min}(x,z)\geq\min\{n_{\min}(x,y),n_{\min}(y,z)\},
$$

and therefore

$$
d(x,z)\leq\max\{d(x,y),d(y,z)\}\leq d(x,y)+d(y,z).
$$

**Thus $d$ is a [metric](../../../../../../metric.md); in fact, the stronger first inequality makes it an [ultrametric](../../../../../../ultrametric.md).**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12G](../../12g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

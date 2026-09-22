<h1 id="9e/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [sequence](../../../../../../sequence.md) converges to $\ell$ precisely when

$$
\boxed{\forall\varepsilon>0\ \exists N\in\mathbb N\ \forall n\geq N:\quad |x_n-\ell|<\varepsilon.}
$$

For a finite collection of [convergent sequences](../../../../../../convergent-sequence.md), choose $N_j$ for the same tolerance $\varepsilon$ in row $j$, and let $N=\max_{1\leq j\leq k}N_j$. If $n\geq N$, every available $y_n^{(j)}$ lies within $\varepsilon$ of $\ell$, and so does any selected $x_n$. **Every such finite rowwise selection converges to $\ell$**. The finiteness is what permits a single maximum of the cutoffs.

For the infinite collection, define

$$
\boxed{y_n^{(j)}=\begin{cases}\ell+(-1)^j,&n=j,\\\ell,&n\ne j.\end{cases}}
$$

For every fixed $j$, this [sequence](../../../../../../sequence.md) is eventually exactly $\ell$, and hence converges to $\ell$. But its diagonal selection is $x_n=y_n^{(n)}=\ell+(-1)^n$, which has two distinct subsequential limits and **does not converge**. A moving row index can always choose the exceptional entry before that row reaches its eventual behavior.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9E](../../9e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

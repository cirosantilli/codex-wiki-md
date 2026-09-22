<h1 id="2f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix $\epsilon>0$. For each $N$, the set $Q_N=\bigcap_{n,m\geq N}\{x:|f_n(x)-f_m(x)|\leq\epsilon\}$ is [closed](../../../../../../closed-set.md), because each $f_n-f_m$ is [continuous](../../../../../../continuous-function.md). At every $x$, [pointwise convergence](../../../../../../pointwise-convergence.md) makes $(f_n(x))$ a [Cauchy sequence](../../../../../../cauchy-sequence.md), so $\mathbb R=\bigcup_{N\geq1}Q_N$. The [Baire category theorem](../../../../../../baire-category-theorem.md) supplies an $N_0$ for which $Q_{N_0}$ contains a nonempty [open interval](../../../../../../open-interval.md) $I$. For $x\in I$ and $n\geq N_0$, pass $m\to\infty$ in $|f_n(x)-f_m(x)|\leq\epsilon$ to obtain

$$
\boxed{|f_n(x)-f(x)|\leq\epsilon\quad(x\in I,\ n\geq N_0).}
$$

This [local uniform Cauchy control for pointwise convergent continuous functions](../../../../../../local-uniform-cauchy-control-for-pointwise-convergent-continuous-functions.md) allows both $I$ and $N_0$ to depend on $\epsilon$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2F](../../2f.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

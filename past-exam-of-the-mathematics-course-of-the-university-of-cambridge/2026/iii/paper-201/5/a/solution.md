<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D\subset\mathbb R^d$ be bounded, choose $R$ with $D\subset B(0,R)$, and let $T$ and $\tau_R$ be the respective [exit times](../../../../../../brownian-exit-time.md). Then $T\leq\tau_R$. Since

$$
|B_t|^2-dt
$$

is a [martingale](../../../../../../martingale-split.md), the [optional sampling theorem for a supermartingale](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) at $\tau_R\wedge n$ gives

$$
d\,\mathbb E_x(\tau_R\wedge n)
=\mathbb E_x|B_{\tau_R\wedge n}|^2-|x|^2
\leq R^2-|x|^2.
$$

[Monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) now gives

$$
\boxed{\mathbb E_xT\leq\mathbb E_x\tau_R
\leq\frac{R^2-|x|^2}{d}<\infty.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

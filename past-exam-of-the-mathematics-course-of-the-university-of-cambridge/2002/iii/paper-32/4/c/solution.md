<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Differentiate the negative-root equation $F(\beta_-,\delta)=0$, keeping $r$ and $\sigma$ fixed. Its derivatives are $F_\delta=-\beta_-$ and

$$
F_\beta=\sigma^2\beta_-+r-\delta-\sigma^2/2=-\Delta<0.
$$

Thus $d\beta_-/d\delta=\beta_-/F_\beta=-\beta_-/\Delta>0$. Differentiating the trigger ratio then gives

$$
\boxed{\frac{dS^*}{d\delta}=-\frac{X}{(\beta_--1)^2}\frac{d\beta_-}{d\delta}
=\frac{X\beta_-}{\Delta(\beta_--1)^2}<0.}
$$

This is the [dividend-yield sensitivity of the perpetual put trigger](../../../../../../dividend-yield-sensitivity-of-the-perpetual-put-trigger.md). A larger dividend yield lowers the risk-neutral drift of the ex-dividend [stock](../../../../../../stock.md); waiting for further price reductions becomes more attractive to the put holder, so exercise occurs at a lower price. As checks, at $\delta=0$ the negative root is $-2r/\sigma^2$, giving $S^*=2rX/(2r+\sigma^2)$. As $\delta\to\infty$, $\beta_-\to0-$ and $S^*\to0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

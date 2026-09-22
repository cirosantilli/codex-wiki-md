<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Gumbel distribution](../../../../../../gumbel-distribution.md) for maxima has [distribution function](../../../../../../cumulative-distribution-function.md) $G(x)=\exp(-e^{-x})$ on the whole real line. For $n\geq2$ set

$$
\boxed{\beta_n=(\log n)^2,\qquad \alpha_n=2\log n.}
$$

Both the centering and scale are elementary, and the scale is positive. For any fixed real $x$, the normalized threshold $\beta_n+\alpha_nx$ is positive for all sufficiently large $n$. Writing $L=\log n$, a [Taylor expansion](../../../../../../taylor-expansion.md) gives

$$
\sqrt{\beta_n+\alpha_nx}
=L\sqrt{1+\frac{2x}{L}}
=L+x+O(L^{-1}).
$$

Consequently,

$$
n\overline F(\beta_n+\alpha_nx)
=n\exp\!\left(-\sqrt{\beta_n+\alpha_nx}\right)
\longrightarrow e^{-x}.
$$

The logarithm calculation in part (i) now gives

$$
\boxed{F(\alpha_nx+\beta_n)^n\longrightarrow\exp(-e^{-x})\quad(x\in\mathbb R).}
$$

Thus $F$ belongs to the [maximum domain of attraction](../../../../../../maximum-domain-of-attraction.md) of the standard [Gumbel distribution](../../../../../../gumbel-distribution.md). The scale also has the [Gumbel auxiliary function](../../../../../../gumbel-auxiliary-function.md) interpretation: the reciprocal [hazard function](../../../../../../hazard-function.md) is $2\sqrt t$, whose [derivative](../../../../../../derivative.md) $1/\sqrt t$ tends to zero at the infinite right endpoint. This agrees with the [Von Mises conditions for extreme values](../../../../../../von-mises-conditions-for-extreme-values.md), and at $t=\beta_n$ gives exactly $\alpha_n=2\log n$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

<h1 id="3/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Put $h=\Delta x$. The spatial operator is the sum of a centred $x$ difference and a [dissipative second-order forward advection stencil](../../../../../../dissipative-second-order-forward-advection-stencil.md) in $y$. For a smooth function, their [Taylor expansions](../../../../../../taylor-expansion.md) give

$$
\frac{u(x+h,y)-u(x-h,y)}{2h}
=u_x+\frac{h^2}{6}u_{xxx}+O(h^4),
$$



$$
\frac{-3u(x,y)+4u(x,y+h)-u(x,y+2h)}{2h}
=u_y-\frac{h^2}{3}u_{yyy}-\frac{h^3}{4}u_{yyyy}+O(h^4).
$$

Thus the leading spatial [local truncation error](../../../../../../local-truncation-error.md) is $h^2(u_{xxx}/6-u_{yyy}/3)$, generally nonzero. **The semidiscretization is second order in space.** Time has not yet been discretized, so there is no separate time order or time-step condition at this stage.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [3](../../3.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

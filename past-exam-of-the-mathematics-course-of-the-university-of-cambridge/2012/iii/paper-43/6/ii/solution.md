<h1 id="6/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under the [Black-Scholes model](../../../../../../black-scholes-model.md) pricing measure, write $\log S_t/\sigma=B_t+ct$, where $c=(r-\sigma^2/2)/\sigma$. Brownian continuity and immediate crossing on reaching a level make the strict up-crossing time equal almost surely to the hitting time $H_a$. Its finite-time law has no atom at $T$, so the convention before rather than at expiry does not affect the price.

For [truncated discounted Brownian first passage](../../../../../../truncated-discounted-brownian-first-passage.md), since payment occurs at the hitting time, discount there, not at expiry. The [one-touch option](../../../../../../one-touch-option.md) price is

$$
V_0=\mathbb E[e^{-rH_a}\mathbf1\{H_a\leq T\}]=\int_0^T e^{-rt}h_c(t)dt.
$$

Set $d=\sqrt{c^2+2r}=|r+\sigma^2/2|/\sigma$. The expression under the square root is nonnegative for every real $r$, by this Black-Scholes identity. The discounted density satisfies $e^{-rt}h_c(t)=e^{a(c-d)}h_d(t)$. Applying part i yields **the closed price**

$$
\boxed{V_0=e^{a(c-d)}\Phi\left(\frac{dT-a}{\sqrt T}\right)+e^{a(c+d)}\Phi\left(\frac{-a-dT}{\sqrt T}\right).}
$$

This formula also covers $d=0$ and negative rates. When $r\geq0$, one may use $d=(r+\sigma^2/2)/\sigma$, so the two prefactors simplify to $e^{-\sigma a}$ and $e^{2ra/\sigma}$. At $r=0$ the expression is the undiscounted hitting probability, as a consistency check.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6](../../6.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

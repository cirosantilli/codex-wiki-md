<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For [claim dividends proportional to the underlying stock](../../../../claim-dividends-proportional-to-the-underlying-stock.md), put $V(S,t)=S\phi(t)$. Then $V_S=\phi$, $V_{SS}=0$ and $V_t=S\phi'$, so the [partial differential equation](../../../../partial-differential-equation-split.md) reduces to the [linear ordinary differential equation](../../../../linear-ordinary-differential-equation-split.md)

$$
\phi'-D\phi=-f(t),\qquad\phi(T)=1.
$$

The [integrating factor](../../../../integrating-factor.md) $e^{-Dt}$ gives $(e^{-Dt}\phi)'=-e^{-Dt}f(t)$. Integrating backwards from the terminal value,

$$
\boxed{V(S,t)=S\left[e^{-D(T-t)}+\int_t^T e^{-D(u-t)}f(u)\,du\right]}.
$$

The formula assumes the displayed [integral](../../../../integral-split.md) is finite. Under the [risk-neutral measure](../../../../risk-neutral-measure.md), $\mathbb E_t[S_u]=S e^{(r-D)(u-t)}$. Discounting each cash payment at its own payment time gives the same result:

$$
V=\mathbb E_t\!\left[e^{-r(T-t)}S_T+\int_t^T e^{-r(u-t)}f(u)S_u\,du\right].
$$

The [interest rate](../../../../interest-rate.md) disappears because every payment is proportional to the [stock](../../../../stock.md) price.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical models of financial derivatives course of the University of Oxford](../../../split.md)
5. [Mathematical models of financial derivatives course of the University of Oxford](../../../../mathematical-models-of-financial-derivatives-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

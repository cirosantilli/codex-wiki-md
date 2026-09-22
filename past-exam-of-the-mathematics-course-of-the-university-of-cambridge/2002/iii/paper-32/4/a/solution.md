<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $r>0$, $\sigma>0$ and proportional [continuous dividend yield](../../../../../../continuous-dividend-yield.md) $\delta\ge0$, the usual perpetual-option setting. Write $L$ for the prescribed downward exercise trigger, with $0<L<X$. Above the trigger there is no dependence on calendar time, so the [Black-Scholes equation with continuous stock dividends](../../../../../../black-scholes-equation-with-continuous-stock-dividends.md) reduces to

$$
\frac12\sigma^2S^2V''+(r-\delta)SV'-rV=0.
$$

Substitute $V=S^\beta$. The characteristic equation and its roots are

$$
F(\beta)=\frac12\sigma^2\beta(\beta-1)+(r-\delta)\beta-r=0,
\qquad \beta_\pm=\frac{-(r-\delta-\sigma^2/2)\pm\Delta}{\sigma^2},
\quad \Delta=\sqrt{(r-\delta-\sigma^2/2)^2+2r\sigma^2}.
$$

Since the root product is $-2r/\sigma^2<0$, $\beta_-<0<\beta_+$. The [boundary condition](../../../../../../boundary-condition.md) $V(S)\to0$ as $S\to\infty$ excludes the positive-power solution. Value matching at the trigger requires $V(L)=X-L$, giving the fixed-rule price

$$
\boxed{V_L(S)=\begin{cases}
X-S,&0<S\le L,\\
(X-L)(S/L)^{\beta_-},&S>L.
\end{cases}}
$$

The lower branch means exercise immediately if the starting price is already below the trigger. Above it, the formula also equals $\mathbb E_Q[e^{-r\tau_L}(X-L)\mathbf1_{\{\tau_L<\infty\}}]$, where $\tau_L$ is the first passage to $L$. To verify this [expectation](../../../../../../expected-value.md), apply [Itô formula](../../../../../../ito-s-lemma.md) to the bounded stopped discounted solution on $S\ge L$; the generator equation makes it a [martingale](../../../../../../martingale-split.md) before the hit, and the residual term on surviving paths vanishes as the time horizon tends to infinity because $r>0$. A fixed trigger is a specified exercise rule, not yet the optimized American price.

## ↑ Ancestors (11)

1. [A](../a.md)
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

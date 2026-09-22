<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume the usual positive initial [stock](../../../../../../stock.md) price and strike, so the logarithm is defined, and interpret $U$ as a classical solution of the displayed [partial differential equation](../../../../../../partial-differential-equation-split.md). For a fixed complex $z$, put $F_t(z)=S_t^zU(t,\sigma_t,z)$, defining $S_t^z=\exp(z\log S_t)$. The [Itô formula](../../../../../../ito-s-lemma.md) for the two [Brownian motions](../../../../../../brownian-motion-split.md) with [correlation coefficient](../../../../../../pearson-correlation-coefficient.md) $\rho$ gives

$$
\begin{aligned}
dF_t(z)=S_t^z\bigg(&U_t+A(\sigma_t)U_\sigma+\frac12B(\sigma_t)^2U_{\sigma\sigma}+\frac12\sigma_t^2z(z-1)U+z\sigma_tB(\sigma_t)\rho U_\sigma\bigg)dt\\
&+S_t^z\bigl(z\sigma_tU\,dW_t^S+B(\sigma_t)U_\sigma\,dW_t^\sigma\bigr).
\end{aligned}
$$

The [partial differential equation](../../../../../../partial-differential-equation-split.md) cancels the entire [drift](../../../../../../drift-coefficient.md). By the permission to treat the resulting [local martingales](../../../../../../local-martingale.md) as true [martingales](../../../../../../martingale-split.md), and the terminal condition, $F_t(z)=\mathbb E[S_T^z\mid\mathcal F_t]$.

The bounded [spot volatility](../../../../../../spot-volatility.md) ensures $\mathbb ES_T^{x_0}<\infty$: the [Itô formula](../../../../../../ito-s-lemma.md) for a real power and localization bound its [moment](../../../../../../moment.md) by $S_0^{x_0}\exp(x_0(x_0-1)\|\sigma\|_\infty^2T/2)$. Rewrite the proposed integrand as

$$
\frac{S_tU(t,\sigma_t,z)}{f(z,\log(K/S_t))}=\frac{K^{1-z}F_t(z)}{z(z-1)}.
$$

Now $|F_t(x_0+iy)|\leq\mathbb E[S_T^{x_0}\mid\mathcal F_t]$, an integrable bound independent of $y$. Conditional [Fubini's theorem](../../../../../../fubini-s-theorem.md) and part (b) therefore imply

$$
\boxed{C_t=\mathbb E[(S_T-K)^+\mid\mathcal F_t].}
$$

This route justifies the contour exchange without assuming bounds on $U$ uniform in all complex $z$. Cash is constant, $S$ is a true [martingale](../../../../../../martingale-split.md) under the stated allowance, and the displayed $C$ is a true [martingale](../../../../../../martingale-split.md). The original measure is thus an [equivalent martingale measure](../../../../../../risk-neutral-measure.md) for all three assets. The [fundamental theorem of asset pricing](../../../../../../fundamental-theorem-of-asset-pricing.md) gives **the market has no [arbitrage](../../../../../../arbitrage.md) under the usual admissible trading convention.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

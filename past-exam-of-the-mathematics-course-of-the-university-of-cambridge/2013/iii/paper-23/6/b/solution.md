<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume [Riemann hypothesis](../../../../../../riemann-hypothesis.md). First fix $0<\delta<1/4$ and work on $\sigma_0=1/2+\delta$. We prove the [subpower zeta bound to the right of the critical line](../../../../../../subpower-zeta-bound-to-the-right-of-the-critical-line.md), then move back to the line by the [functional equation](../../../../../../functional-equation.md) and [Phragmén–Lindelöf principle](../../../../../../phragmen-lindelof-principle.md).

Put $x=\log t$ for large positive $t$ and integrate the supplied smoothed [logarithmic derivative](../../../../../../logarithmic-derivative.md) identity horizontally from $\sigma_0$ to two. There are no zeros on this path under [Riemann hypothesis](../../../../../../riemann-hypothesis.md), so the Euler-product logarithm at $2+it$ continues along it. Each prime-power term contributes at most $\Lambda(n)n^{-\sigma_0}/\log n\le n^{-\sigma_0}$, and the smoothing weights are at most one. Hence the integrated [prime](../../../../../../prime-number.md) terms are bounded by

$$
C_\delta\sum_{n\le x^2}n^{-\sigma_0}\ll_\delta x^{1-2\delta}=o(\log t).
$$

All zeros have $\rho=1/2+i\gamma$. The local zero-count estimate from Question 3, with its reflected version for negative ordinates, gives uniformly for $\sigma_0\le\sigma\le2$

$$
\sum_\rho\frac1{|\rho-\sigma-it|^2}\le C_\delta\log t.
$$

To see the uniformity, sum the $O(\log(2+|\gamma|))$ zeros in successive unit ordinate intervals against $(\delta^2+|t-\gamma|^2)^{-1}$; the distant dyadic tails are summable. The zero-term numerator has modulus at most $x^{-2\delta}+x^{-\delta}$. Its integrated contribution is therefore at most $C_\delta x^{-\delta}\log t/\log x=o(\log t)$. The integrated supplied remainder is $O(x^{-1-\delta}\log t/\log x)$, also $o(\log t)$. Since $\log\zeta(2+it)$ is bounded, we obtain

$$
|\log\zeta(1/2+\delta+it)|=o_\delta(\log t).
$$

Thus for every fixed $\delta>0$ and $\eta>0$, $|\zeta(1/2+\delta+it)|\ll_{\delta,\eta}t^\eta$. Negative $t$ follow by [complex conjugation](../../../../../../complex-conjugation.md).

The zeta [functional equation](../../../../../../functional-equation.md) and the gamma ratio give $|\zeta(1/2-\delta+it)|\ll_{\delta,\eta}t^{\delta+\eta}$. Zeta is [holomorphic](../../../../../../complex-differentiability-at-a-point.md) throughout this strip, since its [pole](../../../../../../pole.md) at one is outside it, and Euler summation supplies [polynomial](../../../../../../polynomial-split.md) vertical growth. The strip convexity conclusion of [Phragmén–Lindelöf principle](../../../../../../phragmen-lindelof-principle.md) therefore gives at the midpoint

$$
|\zeta(1/2+it)|\ll_{\delta,\eta}(1+|t|)^{\delta/2+\eta}.
$$

For a prescribed $\varepsilon>0$, choose $\delta$ and $\eta$ with $\delta/2+\eta<\varepsilon$; the bounded $t$ range is harmless. This proves

$$
\boxed{\text{Riemann hypothesis}\ \Longrightarrow\ \text{Lindelöf hypothesis}.}
$$

The explicit-formula estimate is deliberately first made a fixed distance to the right of the [critical line](../../../../../../critical-line.md). No divergent zero bound at $\sigma=1/2$ is used.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

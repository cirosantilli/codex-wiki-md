# Mellin transform in logarithmic coordinates

↑ **Parent:** [Mellin transform](mellin-transform.md)

The [change of variables](change-of-variables-formula.md) $x=e^u$, using the [exponential function](exponential-function.md), turns the [Mellin transform](mellin-transform.md) into

$$
\mathcal Mf(s)=\int_{-\infty}^\infty e^{su}f(e^u)\,du.
$$

The factor $dx=e^u du$ changes $x^{s-1}$ to $e^{su}$; missing this factor would shift every exponent by one. With $h_\sigma(u)=e^{\sigma u}f(e^u)$ and the [Fourier transform](fourier-transform-split.md) convention $\widehat h(\omega)=\int_{\mathbb R}h(u)e^{-i\omega u}\,du$, the identity is

$$
\mathcal Mf(\sigma+i\tau)=\int_{\mathbb R}h_\sigma(u)e^{i\tau u}\,du=\widehat h_\sigma(-\tau).
$$

Choosing $\sigma$ inside the [Mellin fundamental strip](fundamental-strip-of-a-mellin-transform.md) makes $h_\sigma$ a [Lebesgue integrable function](lebesgue-integrable-function.md). The minus sign in the [Fourier transform](fourier-transform-split.md) argument follows from the stated convention. For the [Mellin transform of an interval indicator](mellin-transform-of-an-interval-indicator.md) with $[b,c]=[1,4]$ and $\sigma=0$, $h_0=\mathbf1_{[0,\log4]}$: the [Fourier transform of an interval indicator](fourier-transform-of-an-interval-indicator.md) is literally the same computation in a different coordinate.

Splitting the [real line](real-line.md) at $u=0$ also connects the [Mellin transform](mellin-transform.md) to two unilateral [Laplace transforms](laplace-transform.md). If $k_+(v)=f(e^v)$ and $k_-(v)=f(e^{-v})$ for $v\geq0$, then

$$
\mathcal Mf(s)=\mathcal Lk_+(-s)+\mathcal Lk_-(s)
$$

where both [integrals](integral-split.md) converge absolutely. Their [Laplace convergence regions](region-of-absolute-convergence-of-a-laplace-transform.md) impose opposite endpoint conditions, explaining the two sides of the [Mellin fundamental strip](fundamental-strip-of-a-mellin-transform.md). Finally, $f(ae^u)=f(e^{u+\log a})$ shows that a change of scale is a [translation](translation-geometry.md) in $u$. Weighted [Fourier transforms](fourier-transform-split.md) of this [translation](translation-geometry.md) give exactly the factor $a^{-s}$ in the [scaling property of the Mellin transform](scaling-property-of-the-mellin-transform.md). For a smooth [function](function-split.md) with [compact support](compact-support.md) inside $(0,\infty)$, the [Mellin inversion theorem](mellin-inversion-theorem.md) follows from [Fourier inversion](fourier-inversion-theorem.md); the existing formula states the corresponding hypotheses.

## ↑ Ancestors (6)

1. [Mellin transform](mellin-transform.md)
2. [Integral transform](integral-transform-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Mellin transform](mellin-transform.md)

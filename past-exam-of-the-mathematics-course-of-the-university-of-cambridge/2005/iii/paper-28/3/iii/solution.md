<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A fixed zero-free strip changes the zero contribution qualitatively. If every nontrivial zero satisfies $\beta<1-c$, with fixed $0<c<1/2$, the same zero-count estimate and [partial summation](../../../../../../abel-s-summation-formula.md) give

$$
\left|\sum_{|\rho|<T}\frac{x^\rho}{\rho}\right|
\ll x^{1-c}\log^2(T+2).
$$

The [truncated explicit formula for the second Chebyshev function](../../../../../../truncated-explicit-formula-for-the-second-chebyshev-function.md) then yields

$$
|\psi(x)-x|\ll x^{1-c}\log^2(T+2)+\frac{x\log^2x}{T}.
$$

Take $T=x^c$, or an admissible height of this size. The two contributions are bounded by the same order, proving the [prime number theorem error from a fixed zero-free strip](../../../../../../prime-number-theorem-error-from-a-fixed-zero-free-strip.md):

$$
\boxed{|\psi(x)-x|=O\bigl(x^{1-c}\log^2x\bigr).}
$$

In particular this is $O_\varepsilon(x^{1-c+\varepsilon})$ for every $\varepsilon>0$. It is a power saving, stronger than the decay obtained from the logarithmic zero-free region. The triangle-inequality estimate of the zero sum explains the two logarithms; removing them would require additional information or cancellation, not merely the asserted zero-free strip.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

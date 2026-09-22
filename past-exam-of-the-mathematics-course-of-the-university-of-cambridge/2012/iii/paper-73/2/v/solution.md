<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let the [two-dimensional enstrophy cascade](../../../../../../two-dimensional-enstrophy-cascade.md) spectrum be $E(k)=Ck^{-3}$ between $k_0$ and $k_d$, and choose a separation well inside the range: $k_0\ll k_c=\pi/r\ll k_d$. The high-wavenumber energy is

$$
\int_{k_c}^{k_d}E(k)\,dk=\frac C2(k_c^{-2}-k_d^{-2})\simeq\frac{Cr^2}{2\pi^2}.
$$

The low-wavenumber correction instead gives

$$
\frac{r^2}{8}\int_{k_0}^{k_c}k^2E(k)\,dk
=\frac{Cr^2}{8}\log\frac{k_c}{k_0}.
$$

Its ratio to the preceding energy contribution is $(\pi^2/4)\log(k_c/k_0)$, which is large when the separation is sufficiently far below the [integral scale of turbulence](../../../../../../integral-scale-of-turbulence.md). Consequently

$$
\boxed{S_2(r)\simeq\frac{Cr^2}{4}\log\frac{\pi}{k_0r}},
$$

up to the stated piecewise-filter approximation and subleading contributions. Equivalently, if $Z_{<k_c}=\int_0^{k_c}k^2E(k)\,dk$ is the cumulative [enstrophy](../../../../../../enstrophy.md) in motions larger than $r$, then $S_2\simeq r^2Z_{<k_c}/4$.

**The leading increment [variance](../../../../../../variance-split.md) is controlled by the accumulated [enstrophy](../../../../../../enstrophy.md) at scales larger than the separation, rather than the [kinetic energy](../../../../../../kinetic-energy.md) at smaller scales.** For a $k^{-3}$ spectrum, each logarithmic wavenumber interval contributes the same amount to that [enstrophy](../../../../../../enstrophy.md) integral, so the conclusion does not mean that only the largest eddy supplies it. The logarithm is a marginal failure of a pure local $r^2$ estimate. The stipulated wide power-law range is essential, and the dominance need not hold at its upper spatial edge where $k_c/k_0$ is only of order one.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

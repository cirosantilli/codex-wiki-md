<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $\widehat{f\sigma}(x)=\int_{S^1}f(\omega)e^{-2\pi ix\cdot\omega}\,d\sigma(\omega)$, with arclength measure. We first bound the transform for constant density. By rotational symmetry, $\widehat\sigma(x)=\int_0^{2\pi}e^{-2\pi ir\cos\theta}d\theta$, $r=|x|$. For $r\geq1$, remove neighborhoods of width $h=r^{-1/2}$ about the stationary points $0,\pi$. Their contribution is $O(h)$. On each remaining interval integrate by parts using the phase derivative $2\pi r\sin\theta$. The boundary terms are $O((rh)^{-1})$, and the integral of the derivative of its reciprocal is bounded by

$$
\frac Cr\int_h^{\pi-h}\frac{|\cos\theta|}{\sin^2\theta}d\theta\lesssim\frac1{rh}.
$$

Splitting at the stationary points gives the same bound on the other half of the circle. Together with the trivial estimate for bounded $r$, this proves $|\widehat\sigma(x)|\lesssim(1+|x|)^{-1/2}$.

For merely measurable $f$ there is no reason that its amplitude permits this [integration by parts](../../../../../integration-by-parts.md). Instead use [Gaussian positivity for even extension moments](../../../../../gaussian-positivity-for-even-extension-moments.md). Set

$$
I_R(f)=\int_{\mathbb R^2}|\widehat{f\sigma}(x)|^4e^{-\pi|x|^2/R^2}dx.
$$

Expand the fourth power and integrate first in $x$. The [Fourier transform of a Gaussian](../../../../../fourier-transform-of-a-gaussian.md) gives

$$
I_R(f)=R^2\int_{(S^1)^4} f(\omega_1)f(\omega_2)\overline{f(\omega_3)f(\omega_4)}\,e^{-\pi R^2|\omega_1+\omega_2-\omega_3-\omega_4|^2}\,d\sigma^4.
$$

All exchanges of integrals are justified by bounded amplitudes, finite surface measure and the integrable Gaussian. The kernel is nonnegative and $|f|\leq1$ almost everywhere. Taking the absolute value of the integral therefore gives $0\leq I_R(f)\leq I_R(1)$. The preceding scalar decay estimate and polar coordinates yield

$$
I_R(1)\lesssim\int_0^\infty\frac{r}{(1+r)^2}e^{-\pi r^2/R^2}dr\lesssim1+\log R\lesssim\log R\qquad(R\geq2).
$$

For the last bound split at $1$ and $R$; the tail becomes an integrable $e^{-\pi s^2}/s$ integral after $r=Rs$. Since the Gaussian is at least $e^{-\pi}$ on the radius-$R$ ball, the [local fourth-moment restriction estimate for the circle](../../../../../local-fourth-moment-restriction-estimate-for-the-circle.md) follows:

$$
\boxed{\|\widehat{f\sigma}\|_{L^4(B(0,R))}\leq C(\log R)^{1/4}.}
$$

Every constant here is independent of $f$ and $R$.

For the requested connection to [Besicovitch sets](../../../../../besicovitch-set.md), let $\delta$ be small and dilate the unit segments of a bounded planar Kakeya set by $\delta^{-2}$. Their $\delta$-neighborhoods become direction-separated rectangles of length $\delta^{-2}$ and width $\delta^{-1}$. A smooth circle cap of angular width $c\delta$ has a [Fourier extension operator](../../../../../fourier-extension-operator.md) of magnitude at least $c'\delta$ on such a rectangle: after removing the constant phase, the tangential phase variation is $O(c)$ and the normal variation is $O(c^2)$. A frequency modulation translates the rectangle to any desired location. Choose separated caps for the rectangle directions, and multiply their modulated densities by independent [Rademacher random variables](../../../../../rademacher-distribution.md). Because the caps are disjoint, the input remains bounded by one.

Apply the local fourth-moment estimate in a ball of radius $C_E\delta^{-2}$ containing the rectangles, then take expectation over the [Rademacher random variables](../../../../../rademacher-distribution.md). The fourth moment dominates the square of the sum of squared packet magnitudes, giving

$$
\delta^4\int\left(\sum_j1_{T_j}\right)^2\lesssim_E\log(1/\delta).
$$

There are $M\asymp\delta^{-1}$ rectangles, each of area $\asymp\delta^{-3}$, so the integral of their sum is $\asymp\delta^{-4}$. [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) forces their union area to be at least $c_E\delta^{-4}/\log(1/\delta)$. Scaling back gives $|E_{C\delta}|\gtrsim_E1/\log(1/\delta)$, the [planar Kakeya neighborhood lower bound](../../../../../planar-kakeya-neighborhood-lower-bound.md). The covering-number argument in Question 1 then gives both [Minkowski dimensions](../../../../../box-counting-dimension.md) equal to two.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

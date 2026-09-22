# Jump response of a localized analyzing function

↑ **Parent:** [Vanishing moment](vanishing-moment.md)

Let $\psi$ be an [integrable function](lebesgue-integrable-function.md) with at least one [vanishing moment](vanishing-moment.md). For a unit [jump discontinuity](jump-discontinuity.md) $f(x)=H(x-x_0)$, where $H$ is the [Heaviside step function](heaviside-step-function.md), substitution into the coefficient gives

$$
c_\psi(f;a,b)=\sqrt a\int_\theta^\infty\overline{\psi(u)}\,du,\qquad\theta=\frac{x_0-b}{a}.
$$

The signed [integral](integral.md) of the whole analyzing [function](function-split.md) is zero, but the [jump discontinuity](jump-discontinuity.md) cuts through its [support of a function](support.md) and usually leaves an unbalanced partial [integral](integral.md). At fixed relative position $θ$ with nonzero partial [integral](integral.md), the coefficient decays as $\sqrt a$, slower than the $a^{q+1/2}$ [Taylor remainder](taylor-remainder.md) bound on a [smooth](smooth-function.md) region. “Edges survive” means this relative contrast: the normalized coefficients still tend to zero as $a\to0$.

For an original exact comparison, use the [smooth](smooth-function.md) [polynomial](polynomial-split.md) $f(x)=x+x^2$ at $b=0$. The [Haar wavelet](haar-wavelet.md) $h$ and the [second-difference analyzing function](second-difference-analyzing-function.md) $η$ give

$$
c_h(f;a,0)=-\frac{a^{3/2}+a^{5/2}}4,\qquad c_\eta(f;a,0)=\frac2{\sqrt6}a^{5/2}.
$$

The linear term cancels for $η$; it remains for $h$. For the fixed unit [jump discontinuity](jump-discontinuity.md) $H(x)$, choose $b=-a/4$ so that $θ=1/4$ at every scale. Then

$$
c_h(H;a,-a/4)=-\frac{\sqrt a}{4},\qquad c_\eta(H;a,-a/4)=-\frac{\sqrt a}{4\sqrt6}.
$$

<a id="image-exact-normalized-detail-coefficients-across-scales-for-a-smooth-polynomial-and-a-fixed-unit-jump"></a>
![](wavelet-smooth-jump-scale-coefficients.png)

**[Figure 4](#image-exact-normalized-detail-coefficients-across-scales-for-a-smooth-polynomial-and-a-fixed-unit-jump). Exact normalized detail coefficients across scales for a smooth polynomial and a fixed unit jump**.

Position matters. If an analyzing [function](function-split.md)'s [support of a function](support.md) lies entirely on one constant side of the [jump discontinuity](jump-discontinuity.md), its coefficient is zero. Even a crossing can cancel: $η$ has zero partial [integral](integral.md) at $θ=3/2$. A [jump discontinuity](jump-discontinuity.md) on a [dyadic interval](dyadic-interval.md) boundary can likewise escape finer [Haar wavelets](haar-wavelet.md) whose [supports](support.md) do not cross it. These examples describe particular [functions](function-split.md) and normalizations, not a universal ranking of [wavelets](wavelet.md) for [signal processing](signal-processing.md).

## ↑ Ancestors (7)

1. [Vanishing moment](vanishing-moment.md)
2. [Wavelet](wavelet.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Vanishing moment](vanishing-moment.md)

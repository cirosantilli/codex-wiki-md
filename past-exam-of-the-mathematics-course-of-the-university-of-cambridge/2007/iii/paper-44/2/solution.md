<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $K(t)=\log\mathbb E[e^{tY}]$ for the [cumulant-generating function](../../../../../cumulant-generating-function.md) in the question's $(\phi,\lambda)$ parametrization. Multiplying the density by $e^{ty}$ replaces $\phi$ in the decaying part of its exponent by $\phi-2t$. For $t<\phi/2$, the remaining integral is the normalizing integral for an [Inverse Gaussian distribution](../../../../../inverse-gaussian-distribution.md) with parameters $(\phi-2t,\lambda)$. Comparing the two normalizing constants gives

$$
\mathbb E[e^{tY}]=\exp\{\sqrt{\lambda\phi}-\sqrt{\lambda(\phi-2t)}\},\qquad K(t)=\sqrt{\lambda\phi}-\sqrt{\lambda(\phi-2t)}.
$$

In particular $K'(0)=\sqrt{\lambda/\phi}$, so the mean parameter used in the more usual [Inverse Gaussian distribution](../../../../../inverse-gaussian-distribution.md) notation is $\mu=\sqrt{\lambda/\phi}$; it must not be confused with the present parameter $\phi$.

First compute the [cumulant-generating function](../../../../../cumulant-generating-function.md) of the sample average, as requested. Independence gives

$$
K_{\overline Y_n}(t)=nK(t/n)=n\sqrt{\lambda\phi}-n\sqrt{\lambda(\phi-2t/n)}.
$$

This is exactly the [cumulant-generating function](../../../../../cumulant-generating-function.md) of an [Inverse Gaussian distribution](../../../../../inverse-gaussian-distribution.md) with parameters $(n\phi,n\lambda)$. The [uniqueness theorem for moment-generating functions](../../../../../uniqueness-theorem-for-moment-generating-functions.md) therefore identifies that law. Scaling $S_n=n\overline Y_n$ and including the density Jacobian $1/n$ gives

$$
\boxed{f_{S_n}(s)=\frac{n\sqrt\lambda}{\sqrt{2\pi}s^{3/2}}\exp\left[n\sqrt{\lambda\phi}-\frac12\left(\frac{n^2\lambda}{s}+\phi s\right)\right],\qquad s>0.}
$$

Equivalently, the [inverse Gaussian sum closure](../../../../../inverse-gaussian-sum-closure.md) is $S_n\sim IG(\phi,n^2\lambda)$ in the parametrization of this question. Its mean is $n\sqrt{\lambda/\phi}$ and its [variance](../../../../../variance-split.md) is $n\sqrt\lambda/\phi^{3/2}$, in agreement with addition of independent means and variances.

For a general continuous iid sample with [cumulant-generating function](../../../../../cumulant-generating-function.md) $K$, finite near zero, set $x=s/n$ and choose a real saddle $\widehat t$ in the interior of the finite moment domain satisfying $K'(\widehat t)=x$. With $K''(\widehat t)>0$, the [saddlepoint density approximation](../../../../../saddlepoint-density-approximation.md) for the sum is

$$
\boxed{\widehat f_{S_n}(s)=\frac{\exp\{n[K(\widehat t)-\widehat t x]\}}{\sqrt{2\pi nK''(\widehat t)}}.}
$$

Under the usual smooth nonlattice conditions, at a fixed interior $x$ the true density has this leading expression times $1+O(n^{-1})$. This is a relative density approximation; the leading expression is not automatically an exactly normalized probability density in every model.

One way to understand the [statistical saddlepoint approximation](../../../../../saddlepoint-density-approximation.md) is through [exponential tilting](../../../../../exponential-tilting.md). The tilted one-observation density is $f_t(y)=e^{ty-K(t)}f(y)$, with mean $K'(t)$ and [variance](../../../../../variance-split.md) $K''(t)$. Undoing this tilt for the sum multiplies its tilted density at $s$ by $e^{nK(t)-ts}$. At $t=\widehat t$, $s$ is exactly the tilted mean of the sum. A local version of the [central limit theorem](../../../../../central-limit-theorem.md) gives tilted density there approximately $[2\pi nK''(\widehat t)]^{-1/2}$. Multiplying these two factors gives the displayed [saddlepoint density approximation](../../../../../saddlepoint-density-approximation.md). Higher local expansion terms produce the stated relative error order.

For the [Inverse Gaussian distribution](../../../../../inverse-gaussian-distribution.md), differentiation gives

$$
K'(t)=\frac{\sqrt\lambda}{\sqrt{\phi-2t}},\qquad K''(t)=\frac{\sqrt\lambda}{(\phi-2t)^{3/2}}.
$$

Thus for every $x>0$ the saddle exists, with

$$
\widehat t=\frac12\left(\phi-\frac{\lambda}{x^2}\right)<\frac\phi2,\qquad K''(\widehat t)=\frac{x^3}{\lambda}.
$$

At this saddle,

$$
K(\widehat t)-\widehat t x=\sqrt{\lambda\phi}-\frac12\left(\frac\lambda x+\phi x\right).
$$

Substitution into the [saddlepoint density approximation](../../../../../saddlepoint-density-approximation.md) gives precisely the exact density already found for $S_n$. Therefore

$$
\boxed{\widehat f_{S_n}(s)=f_{S_n}(s)\quad\text{for every }s>0\text{ and every }n\geq1.}
$$

This [exact saddlepoint density of an inverse Gaussian sum](../../../../../exact-saddlepoint-density-of-an-inverse-gaussian-sum.md) is stronger than a relative $O(n^{-1})$ claim: the leading formula is exact and needs no renormalization.

For the final distribution, both tails decay polynomially. Any positive exponential tilt makes the positive tail nonintegrable, and any negative tilt makes the negative tail nonintegrable. Its [moment-generating function](../../../../../moment-generating-function.md) is therefore infinite away from zero, leaving no open interval on which to form the [cumulant-generating function](../../../../../cumulant-generating-function.md) and solve a saddle equation. Here [polynomial tails prevent exponential tilting](../../../../../polynomial-tails-prevent-exponential-tilting.md), so the conventional [saddlepoint density approximation](../../../../../saddlepoint-density-approximation.md) is unavailable. A finite mean and [variance](../../../../../variance-split.md), and even an ordinary [central limit theorem](../../../../../central-limit-theorem.md), do not supply the missing exponential moments.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 44](../../paper-44-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

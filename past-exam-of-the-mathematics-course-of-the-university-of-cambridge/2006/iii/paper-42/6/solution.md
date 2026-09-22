<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $c=g''(\widetilde y)>0$. Near the interior minimum, [Taylor expansion](../../../../../taylor-expansion.md) gives

$$
g(y)=g(\widetilde y)+\tfrac12c(y-\widetilde y)^2+O((y-\widetilde y)^3).
$$

On the scale $y=\widetilde y+z/\sqrt{nc}$, the leading exponent is $ng(\widetilde y)+z^2/2$ and $dy=dz/\sqrt{nc}$. If the integral is localized at this minimum, the rescaled integration endpoints tend to infinity in both directions, so the [Gaussian integral](../../../../../gaussian-integral.md) gives [Laplace's method](../../../../../laplace-s-method.md):

$$
\boxed{\int_a^b e^{-ng(y)}\,dy=e^{-ng(\widetilde y)}\sqrt{\frac{2\pi}{n g''(\widetilde y)}}\{1+O(n^{-1})\}.}
$$

Formally expanding the cubic term gives an order-$n^{-1/2}$ correction odd in $z$, whose [Gaussian integral](../../../../../gaussian-integral.md) is zero. Quartic terms and the square of the cubic term produce the order-$n^{-1}$ correction. Sufficient smoothness near the minimum and control of the exterior integral justify this formal calculation.

**The printed local assumptions alone do not guarantee localization.** A useful [localization condition for Laplace's method](../../../../../localization-condition-for-laplace-s-method.md) is that $g(y)\geq g(\widetilde y)+\delta_\varepsilon$ outside each sufficiently small fixed neighbourhood of $\widetilde y$, for some $\delta_\varepsilon>0$, and that $\int_a^b e^{-n_*g(y)}\,dy<\infty$ for some $n_*>0$. For $n>n_*$, the exterior contribution is at most

$$
e^{-(n-n_*)\{g(\widetilde y)+\delta_\varepsilon\}}\int_a^b e^{-n_*g(y)}\,dy,
$$

which is exponentially smaller than the displayed local term. To see why something of this kind is needed, take $g(y)=y^2(1-y)^4$ on $(-1,1)$. Its unique minimum is at zero and $g''(0)=2$, yet on $1-n^{-1/4}<y<1$ we have $ng(y)\leq1$. This boundary interval alone contributes at least $e^{-1}n^{-1/4}$, dominating the proposed $n^{-1/2}$ local approximation. The Laplace formula therefore has its usual implicit tail assumption, rather than following from uniqueness of the interior minimum alone.

For the [gamma function](../../../../../gamma-function.md), set $y=nu$ to obtain

$$
\Gamma(n+1)=n^{n+1}\int_0^\infty e^{-n(u-\log u)}\,du.
$$

Here $g(u)=u-\log u$ has its unique minimum at $u=1$, with $g(1)=1$ and $g''(1)=1$. It tends to infinity at both endpoints, and its integral is finite for positive exponents, so localization holds. [Laplace's method](../../../../../laplace-s-method.md) yields [Stirling's formula](../../../../../stirling-formula.md):

$$
\boxed{\Gamma(n+1)=\sqrt{2\pi n}\left(\frac ne\right)^n\{1+O(n^{-1})\}.}
$$

For a [prior density](../../../../../prior-density.md) $p$ and independent observations, Bayes' theorem writes the desired posterior [expectation](../../../../../expected-value.md) as a ratio of integrals:

$$
\mathbb E[g(\theta)\mid Y]=\frac{\int_\Theta g(\theta)e^{H_n(\theta)}\,d\theta}{\int_\Theta e^{H_n(\theta)}\,d\theta},\qquad H_n(\theta)=\log p(\theta)+\sum_{i=1}^n\log f(Y_i\mid\theta).
$$

Suppose the log-posterior kernel has a unique concentrating interior mode $\widetilde\theta$, with curvature $J_n=-H_n''(\widetilde\theta)>0$ of order $n$, and the smoothness and tail conditions hold for both integrals. Expanding $H_n$ quadratically gives a common Gaussian factor $e^{H_n(\widetilde\theta)}\sqrt{2\pi/J_n}$. Replacing the smooth amplitude $g(\theta)$ by $g(\widetilde\theta)$ gives

$$
\boxed{\mathbb E[g(\theta)\mid Y]=g(\widetilde\theta)+O(n^{-1}).}
$$

This approximation does not require $g$ to be positive: it treats $g$ as an amplitude, without taking its logarithm. For more accuracy, expand the amplitude and the cubic term in the log-posterior kernel. With $s=\theta-\widetilde\theta$, the Gaussian moments are $\mathbb Es^2=J_n^{-1}$ and $\mathbb Es^4=3J_n^{-2}$. Terms multiplying $g(\widetilde\theta)$ cancel between numerator and denominator; the two remaining first corrections are

$$
\mathbb E[g(\theta)\mid Y]=g(\widetilde\theta)+\frac{g''(\widetilde\theta)}{2J_n}+\frac{g'(\widetilde\theta)H_n'''(\widetilde\theta)}{2J_n^2}+o(n^{-1}),
$$

under the stronger smoothness, derivative-scaling and [integrability](../../../../../integrability.md) assumptions needed for this expansion. The first term accounts for the curvature of the amplitude and the second for posterior [skewness](../../../../../skewness.md). This is [posterior expectation by Laplace approximation](../../../../../posterior-expectation-by-laplace-approximation.md). If there are several modes, boundary modes, or nonconcentrating tails, the appropriate separate contributions must be included; a single interior [Gaussian approximation](../../../../../normal-approximation.md) cannot then be assumed.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

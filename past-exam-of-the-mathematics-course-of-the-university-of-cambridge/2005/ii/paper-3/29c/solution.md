<h1 id="29c/solution">Solution</h1>

↑ **Parent:** [29C](../29c.md)

For positive time, convolution with the [heat kernel](../../../../../heat-kernel.md) gives

$$
w(t,x)=(K_t*g)(x),\qquad K_t(x)=(4\pi t)^{-n/2}e^{-|x|^2/(4t)}.
$$

Differentiation under the integral verifies the [heat equation](../../../../../heat-equation.md), and the [approximate identity](../../../../../approximate-identity.md) property gives the initial value. Taking absolute values under the integral and using $e^{-|x-y|^2/(4t)}\leq1$ gives

$$
\boxed{|w(t,x)|\leq(4\pi t)^{-n/2}\|g\|_1.}
$$

The printed inequality omits the modulus even though $g$ is complex-valued. A complex number has no compatible order, so the displayed absolute-value estimate is the meaningful correction.

Substitution of $u=e^{it}v$ reduces the forced [partial differential equation](../../../../../partial-differential-equation-split.md) to $(i-\Delta)v=f$. With the [Fourier transform](../../../../../fourier-transform.md) convention for which $\widehat{\Delta v}=-|\xi|^2\widehat v$, set

$$
\widehat v(\xi)=\frac{\widehat f(\xi)}{i+|\xi|^2}.
$$

The denominator never vanishes for real $\xi$. Every derivative of its reciprocal has at most [polynomial](../../../../../polynomial-split.md) growth, so multiplying a [Schwartz function](../../../../../schwartz-function.md) by it gives another [Schwartz function](../../../../../schwartz-function.md). The inverse [Fourier transform](../../../../../fourier-transform.md) therefore supplies the required $v$.

For the prescribed initial value the full solution is $u(t,x)=e^{it}v(x)+K_t*(g-v)(x)$. Applying the [heat kernel](../../../../../heat-kernel.md) estimate to the [Schwartz function](../../../../../schwartz-function.md) $g-v$ proves the stronger uniform conclusion

$$
\boxed{\sup_x|u(t,x)-e^{it}v(x)|\leq(4\pi t)^{-n/2}\|g-v\|_1\longrightarrow0.}
$$

## ↑ Ancestors (10)

1. [29C](../29c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $\theta>0$, $E_s=\exp(\theta B_s-\theta^2s/2)$ is an [Exponential martingale for Brownian motion](../../../../../exponential-martingale-for-brownian-motion.md), as follows directly from [independent](../../../../../independent-random-variables.md) [Gaussian](../../../../../normal-distribution.md) increments. Stop it at $\tau_\delta\wedge t$, where $\tau_\delta$ is the first time $B$ reaches $\delta$. On $\{\tau_\delta\le t\}$,

$$
E_{\tau_\delta}\ge\exp(\theta\delta-\theta^2t/2).
$$

The stopped [expectation](../../../../../expected-value.md) is one and the other contribution is nonnegative, so

$$
\mathbb P(\sup_{s\le t}B_s\ge\delta)\le e^{-\theta\delta+\theta^2t/2}.
$$

For $t>0$, minimize the exponent at $\theta=\delta/t$. Apply the same argument to $-B$ and use the union bound to obtain

$$
\boxed{\mathbb P(\sup_{s\le t}|B_s|>\delta)\le2e^{-\delta^2/(2t)}.}
$$

At $t=0$ the [probability](../../../../../probability.md) is zero; the right side can be interpreted by its limit. This proves the [Gaussian maximal bound for Brownian motion](../../../../../gaussian-maximal-bound-for-brownian-motion.md) without losing an extra factor from a two-sided reflection argument.

Let $L$ be a global Lipschitz constant of $b$. Realize the diffusion with the stated generator by $dX_s^\varepsilon=b(X_s^\varepsilon)ds+\varepsilon dW_s$, where $W$ is a standard $d$-dimensional [Brownian motion](../../../../../brownian-motion-split.md). Global Lipschitz [continuity](../../../../../continuous-function.md) gives existence and uniqueness; its generator is exactly the printed operator. Couple it with the ordinary differential equation having the same initial value $x(0)=x_0$. Subtraction gives, with $D_t=\sup_{s\le t}|X_s^\varepsilon-x_s|$,

$$
D_t\le\varepsilon\sup_{s\le t}|W_s|+L\int_0^tD_sds.
$$

The [Gronwall inequality](../../../../../gronwall-inequality.md) implies $D_t\le\varepsilon e^{Lt}\sup_{s\le t}|W_s|$. If a [Euclidean norm](../../../../../euclidean-norm.md) exceeds $u$, some coordinate has absolute value exceeding $u/\sqrt d$. The scalar bound and a union over the coordinates therefore give

$$
\mathbb P(D_t>\delta)\le2d\exp\!\left(-\frac{\delta^2e^{-2Lt}}{2dt\varepsilon^2}\right),\qquad t>0.
$$

Taking the [logarithm](../../../../../logarithm.md) and multiplying by $\varepsilon^2$ yields the explicit answer

$$
\boxed{\limsup_{\varepsilon\downarrow0}\varepsilon^2\log\mathbb P(D_t>\delta)\le-\frac{\delta^2e^{-2Lt}}{2dt}<0.}
$$

For $t=0$ the [probability](../../../../../probability.md) is zero and the limit is $-\infty$, with $\log0=-\infty$. This is [exponential small-noise concentration for a Lipschitz diffusion](../../../../../exponential-small-noise-concentration-for-a-lipschitz-diffusion.md).

**Matching the deterministic initial value is necessary.** The printed last line specifies the differential equation but does not separately write this initial condition. Without it, take $b=0$ and a deterministic solution displaced from $x_0$ by $2\delta$ in one fixed direction. The deviation event already holds at time zero, giving logarithmic rate zero instead of a strictly negative rate.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)

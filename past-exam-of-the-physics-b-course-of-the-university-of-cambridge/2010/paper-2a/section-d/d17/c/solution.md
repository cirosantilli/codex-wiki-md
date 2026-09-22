<h1 id="section-d/d17/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**[Convolution](../../../../../../convolution.md) describes the response of a [linear time-invariant system](../../../../../../linear-time-invariant-system.md) to an arbitrary input.** If $h$ is its [impulse response](../../../../../../impulse-response.md) and $f$ its input,

$$
\boxed{g(t)=(h*f)(t)=\int_{-\infty}^{\infty}h(t-\tau)f(\tau)\,d\tau.}
$$

This is a weighted sum of responses to shifted [impulses](../../../../../../impulse.md). For integrable [functions](../../../../../../function-split.md) the operation is commutative and associative. A causal system has $h(t)=0$ for $t<0$, restricting the [integral](../../../../../../integral-split.md) to past inputs. With the Fourier convention $F(\omega)=\int f(t)e^{-i\omega t}dt$, the [convolution theorem](../../../../../../convolution-theorem.md) gives $G=HF$.

For example, an [RC low-pass frequency response](../../../../../../rc-low-pass-frequency-response.md) has $h(t)=\tau_0^{-1}e^{-t/\tau_0}\Theta(t)$ and $H(\omega)=(1+i\omega\tau_0)^{-1}$, where $\Theta$ is the [Heaviside step function](../../../../../../heaviside-step-function.md). Fast input variations are smoothed. The same mathematics describes optical blurring by a [point spread function](../../../../../../point-spread-function-split.md) and many other [linear response](../../../../../../linear-response-theory.md) measurements.

[Deconvolution](../../../../../../deconvolution.md) tries to recover $f$ from measured $g$ and known $h$. In noise-free data one formally sets $F=G/H$ where $H\ne0$. Zeros of $H$ lose corresponding information; small values amplify measurement [noise](../../../../../../noise-signal-processing.md). If the measured spectrum is $G+N$, the direct estimate has error $N/H$, which can be very large at [frequencies](../../../../../../frequency.md) strongly suppressed by the instrument. An inverse is therefore not automatically unique or stable.

One [regularized spectral deconvolution](../../../../../../regularized-spectral-deconvolution.md) reconstruction is

$$
\boxed{F_\lambda(\omega)=\frac{H(\omega)^*G(\omega)}{|H(\omega)|^2+\lambda},\qquad\lambda>0.}
$$

This minimizes $|HF-G|^2+\lambda|F|^2$ at each [frequency](../../../../../../frequency.md) and limits [noise](../../../../../../noise-signal-processing.md) amplification, at the cost of bias and lost resolution. Choosing the regularization requires assumptions about [noise](../../../../../../noise-signal-processing.md) and the desired [signal](../../../../../../signal.md); [deconvolution](../../../../../../deconvolution.md) cannot restore components that the data do not determine without such additional information.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [D17](../../d17.md)
3. [Section D](../../../section-d.md)
4. [Paper 2A](../../../../paper-2a-split.md)
5. [2010](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)

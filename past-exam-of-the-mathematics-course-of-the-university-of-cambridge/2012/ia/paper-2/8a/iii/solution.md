<h1 id="8a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [step response of a damped oscillator](../../../../../../step-response-of-a-damped-oscillator.md) is the time integral of its [causal Green function of a damped oscillator](../../../../../../causal-green-function-of-a-damped-oscillator.md). Put $s=t-b$ and define $K(s)=\int_0^s e^{-ku}\sin(\omega u)/\omega\,du$ for $s\geq0$. Then $K(0)=K'(0)=0$ and its oscillator equation has constant right side $1$. Integrating explicitly gives

$$
\boxed{y_3(t,b)=\frac{H(t-b)}{k^2+\omega^2}\left\{1-e^{-k(t-b)}\left[\cos\omega(t-b)+\frac k\omega\sin\omega(t-b)\right]\right\}}.
$$

This formula applies when $\omega\ne0$. It is a [convolution](../../../../../../convolution.md) of the causal impulse response with the shifted [Heaviside step function](../../../../../../heaviside-step-function.md), so the response is zero before the forcing starts and has the stated zero initial data.

The integral definition also handles the degenerate parameters without division ambiguities. For $\omega=0,k\ne0$,

$$
y_3=H(s)\frac{1-e^{-ks}(1+ks)}{k^2};
$$

for $\omega=k=0$, $y_3=H(s)s^2/2$. These are the continuous zero-frequency limits of the step response.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [8A](../../8a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

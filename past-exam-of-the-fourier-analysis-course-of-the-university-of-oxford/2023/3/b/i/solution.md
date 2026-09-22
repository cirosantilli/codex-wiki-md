<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Splitting the [Fourier transform](../../../../../fourier-transform-split.md) integral at zero gives two absolutely convergent [integrals](../../../../../integral-split.md):

$$
\begin{aligned}
\widehat{g_t}(\xi)
&=\int_0^\infty e^{-(t+i\xi)x}\,dx+\int_0^\infty e^{-(t-i\xi)x}\,dx\\
&=\frac1{t+i\xi}+\frac1{t-i\xi}
=\boxed{\frac{2t}{t^2+\xi^2}}.
\end{aligned}
$$

Both $g_t$ and $\widehat{g_t}$ are [integrable functions](../../../../../lebesgue-integrable-function.md). Let $h_t(x)=(t^2+x^2)^{-1}$, so $\widehat{g_t}=2t h_t$. The [duality property of the Fourier transform](../../../../../duality-property-of-the-fourier-transform.md), or [Fourier inversion](../../../../../fourier-inversion-theorem.md) in [tempered distributions](../../../../../tempered-distribution.md), gives

$$
2t\widehat{h_t}(\xi)=\widehat{\widehat{g_t}}(\xi)=2\pi g_t(-\xi).
$$

These [Fourier transforms](../../../../../fourier-transform-split.md) have continuous representatives by the [Riemann-Lebesgue lemma](../../../../../riemann-lebesgue-lemma.md), so the identity holds at every $\xi$. Since $g_t$ is an [even function](../../../../../even-function.md),

$$
\boxed{\mathcal F_{x\to\xi}\!\left(\frac1{t^2+x^2}\right)=\frac\pi t e^{-t|\xi|}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)

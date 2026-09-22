<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Count independent sinusoidal ripples by their spatial [Fourier series](../../../../../../../fourier-series-split.md) indices. A mode with $n$ cycles across $D$ has $\Lambda=D/n$, so the given half-wave index is $j=2n$. The [Nyquist spatial frequency](../../../../../../../nyquist-spatial-frequency.md) permits $n\leq N/2$. In two dimensions, a circular cutoff therefore contains approximately $\pi(N/2)^2$ integer wavevectors.

For a real [wavefront error](../../../../../../../wavefront-error.md), the wavevectors $\mathbf n$ and $-\mathbf n$ describe the same ripple with conjugate coefficients, so count each pair once. The continuum mode-counting approximation gives

$$
\boxed{M\simeq\frac12\pi\left(\frac N2\right)^2=\frac{\pi N^2}8=\frac\pi4\left(\frac{N^2}2\right).}
$$

This counts one ripple with amplitude and phase per conjugate pair, not one real coefficient. Exact finite-grid counts are integers and have boundary corrections; the formula is the circular area estimate implicit in the question, with piston excluded.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 338](../../../../paper-338-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

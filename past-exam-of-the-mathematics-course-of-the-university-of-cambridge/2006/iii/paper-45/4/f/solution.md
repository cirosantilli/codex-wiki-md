<h1 id="4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The rejection rule can use a tighter envelope than 1. For $k>0$, differentiate $\log(e^{-x}x^k/k!)=-x+k\log x-\log(k!)$. Its derivative $-1+k/x$ changes from positive to negative at $x=k$, so

$$
M_k=\sup_{x\ge0}e^{-x}\frac{x^k}{k!}=e^{-k}\frac{k^k}{k!},\qquad M_0=1.
$$

Keep the same joint prior proposal but accept with [probability](../../../../../../probability.md) $w_k(\theta,T)/M_k$. Multiplication of the acceptance function by this constant leaves the accepted [probability density function](../../../../../../probability-density-function.md) unchanged. The improved rate is

$$
\boxed{A_k^{\rm improved}=\frac{Z_k}{M_k}.}
$$

For $k>0$, $M_k<1$, so this is a genuine improvement; for large $k$, [Stirling's formula](../../../../../../stirling-formula.md) gives $M_k\sim(2\pi k)^{-1/2}$. This is the best global constant envelope for an unrestricted positive prior proposal, because $L$ has support $(0,\infty)$ and $\theta L/2$ can approach $k$. For $k=0$ there is no improvement from this constant scaling. Further gains can come from proposals concentrating near $\theta L/2=k$, or integrating out the times first, but such changes require the appropriate proposal-density ratio and envelope rather than an uncorrected alteration of the sampling law.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [4](../../4.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

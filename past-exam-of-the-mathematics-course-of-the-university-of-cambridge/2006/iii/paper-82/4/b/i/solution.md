<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For this sign of the [viscous Burgers equation](../../../../../../../viscous-burgers-equation.md), the [Cole-Hopf transformation](../../../../../../../cole-hopf-transformation.md) is $q=2\delta\partial_\theta\log\psi$. Integrating the initial sinusoid gives $\psi(\theta,0)=C\exp[-\cos\theta/(2\delta)]$; the positive multiplicative constant cancels from $q$. Set $a=1/(2\delta)$ and $s=\delta Z$. The [Fourier series](../../../../../../../fourier-series-split.md) of the initial exponential and the [heat equation](../../../../../../../heat-equation.md) yield the exact [sinusoidal Cole-Hopf solution for negative-flux Burgers flow](../../../../../../../sinusoidal-cole-hopf-solution-for-negative-flux-burgers-flow.md):

$$
\psi(\theta,Z)=I_0(a)+2\sum_{n=1}^{\infty}(-1)^nI_n(a)e^{-n^2s}\cos n\theta.
$$

Each harmonic decays by its heat multiplier, which can also be obtained directly by convolving it with the Gaussian [heat-kernel convolution](../../../../../../../heat-kernel-convolution.md). At $s\gg1$ the first harmonic dominates:

$$
\psi=I_0(a)-2I_1(a)e^{-s}\cos\theta+O(I_0(a)e^{-4s}),\qquad
\psi_\theta=2I_1(a)e^{-s}\sin\theta+O(I_0(a)e^{-4s}).
$$

The error bounds use $|I_n(a)|\le I_0(a)$ for real positive $a$, also immediate from the Fourier-integral representation. Dividing, including the correction from the denominator, gives

$$
q=4\delta\frac{I_1(a)}{I_0(a)}e^{-s}\sin\theta+O(\delta e^{-2s}).
$$

For $\delta\ll1$, the [large-argument asymptotic expansion of a modified Bessel function](../../../../../../../large-argument-asymptotic-expansion-of-a-modified-bessel-function.md) gives $I_1(a)/I_0(a)\to1$. Hence

$$
\boxed{q(\theta,Z)\sim4\delta\sin\theta\,e^{-\delta Z}.}
$$

The sign is positive because the first Fourier harmonic of $\psi$ is negative, so its angular derivative is positive. For a fixed nonzero $\sin\theta$, the relative corrections vanish as $\delta\to0$ and $s\to\infty$; at the symmetry points both the exact solution and the leading expression vanish.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 82](../../../../paper-82-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)

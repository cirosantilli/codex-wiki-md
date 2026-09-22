<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\varepsilon>0$, insert a [Gaussian function](../../../../../gaussian-function.md) into the proposed [inverse Fourier transform](../../../../../inverse-fourier-transform.md):

$$
I_\varepsilon(x)=\frac1{2\pi}\int_{\mathbb R}\widehat\phi(\xi)e^{ix\xi}e^{-\varepsilon\xi^2/2}\,d\xi.
$$

The [Fourier bounds for Schwartz functions](../../../../../fourier-bounds-for-schwartz-functions.md) show that $\widehat\phi$ is an [integrable function](../../../../../lebesgue-integrable-function.md), so [dominated convergence](../../../../../dominated-convergence-theorem.md) gives

$$
I_\varepsilon(x)\longrightarrow\frac1{2\pi}\int_{\mathbb R}\widehat\phi(\xi)e^{ix\xi}\,d\xi.
$$

On the other hand, [Fubini's theorem](../../../../../fubini-s-theorem.md) applies because $\|\phi\|_1\int e^{-\varepsilon\xi^2/2}\,d\xi<\infty$. The given [Fourier transform of a Gaussian](../../../../../fourier-transform-of-a-gaussian.md), rescaled by $\sqrt\varepsilon$, yields

$$
\begin{aligned}
I_\varepsilon(x)
&=\int_{\mathbb R}\phi(y)\left(\frac1{2\pi}\int_{\mathbb R}e^{-\varepsilon\xi^2/2}e^{i(x-y)\xi}\,d\xi\right)dy\\
&=\int_{\mathbb R}\phi(y)\frac{e^{-(x-y)^2/(2\varepsilon)}}{\sqrt{2\pi\varepsilon}}\,dy
=\frac1{\sqrt{2\pi}}\int_{\mathbb R}\phi(x-\sqrt\varepsilon z)e^{-z^2/2}\,dz.
\end{aligned}
$$

The last [integrand](../../../../../integrand.md) is bounded by $\|\phi\|_\infty e^{-z^2/2}/\sqrt{2\pi}$. Since $\phi$ is continuous, another application of [dominated convergence](../../../../../dominated-convergence-theorem.md) makes this tend to $\phi(x)$. Equating the limits proves the [Fourier inversion theorem](../../../../../fourier-inversion-theorem.md):

$$
\boxed{\phi(x)=\frac1{2\pi}\int_{\mathbb R}\widehat\phi(\xi)e^{ix\xi}\,d\xi\qquad(x\in\mathbb R).}
$$

The [Gaussian functions](../../../../../gaussian-function.md) above form an [approximate identity](../../../../../approximate-identity.md); no [Fourier inversion](../../../../../fourier-inversion-theorem.md) was used in evaluating their [integrals](../../../../../integral-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
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
